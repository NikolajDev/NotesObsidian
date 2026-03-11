<%*
const editor = app.workspace.activeLeaf.view.editor;
const cursor = editor.getCursor();
const lineCount = editor.lineCount();

let startLine = -1;
let endLine = -1;

// 1. Find the start of the code block
for (let i = cursor.line; i >= 0; i--) {
    if (editor.getLine(i).startsWith("```python")) {
        startLine = i;
        break;
    }
}

// 2. Find the end of the code block
for (let i = cursor.line; i < lineCount; i++) {
    if (editor.getLine(i).startsWith("```") && i !== startLine) {
        endLine = i;
        break;
    }
}

if (startLine === -1 || endLine === -1) {
    new Notice("Error: Cursor must be inside a ```python code block");
    return;
}

// 3. Extract the code
const code = editor.getRange(
    { line: startLine + 1, ch: 0 },
    { line: endLine, ch: 0 }
);

new Notice("Executing code...");

try {
    const response = await fetch("[https://emkc.org/api/v2/piston/execute](https://emkc.org/api/v2/piston/execute)", {
        method: "POST",
        body: JSON.stringify({
            "language": "python",
            "version": "3.10.0",
            "files": [{ "content": code }]
        })
    });
    
    const data = await response.json();
    const output = data.run.stdout || data.run.stderr || "No output";

    // 4. Place output after the block
    editor.setSelection({ line: endLine, ch: 3 });
    const outputText = `\n\n**Output:**\n\`\`\`text\n${output}\`\`\``;
    editor.replaceSelection(outputText);
    
} catch (e) {
    new Notice("Connection error to Piston API");
}
%>