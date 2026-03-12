# CSS Variables (Custom Properties)

## Description
Reusable values defined once and used anywhere. Defined with `--` prefix.

## Syntax
```css
/* Define variables (usually on :root for global) */
:root {
  --primary: #3498db;
  --secondary: #e74c3c;
  --text: #333;
  --bg: #f5f5f5;
  --radius: 8px;
  --spacing: 16px;
}

/* Use with var() */
.button {
  background-color: var(--primary);
  border-radius: var(--radius);
  padding: var(--spacing);
  color: white;
}

.alert {
  border-left: 4px solid var(--secondary);
  padding: var(--spacing);
}
```

## Dark Mode with Variables
```css
:root {
  --bg: #ffffff;
  --text: #222222;
  --card: #f0f0f0;
}

@media (prefers-color-scheme: dark) {
  :root {
    --bg: #1a1a1a;
    --text: #f0f0f0;
    --card: #2d2d2d;
  }
}

body {
  background: var(--bg);
  color: var(--text);
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    :root {
      --primary: #3498db;
      --secondary: #e74c3c;
      --radius: 8px;
      --spacing: 16px;
    }
    .btn { background: var(--primary); color: white; padding: var(--spacing); border-radius: var(--radius); border: none; cursor: pointer; }
    .alert { border-left: 4px solid var(--secondary); background: #fef0f0; padding: var(--spacing); border-radius: var(--radius); }
    .card { background: white; border-radius: var(--radius); padding: var(--spacing); box-shadow: 0 2px 8px rgba(0,0,0,0.1); }
  </style>
</head>
<body style="font-family: Arial, sans-serif; padding: 20px; background: #f5f5f5; display: flex; flex-direction: column; gap: 12px;">
  <button class="btn">Primary Button</button>
  <div class="alert">Alert using --secondary color and --spacing</div>
  <div class="card">Card using --radius and --spacing variables</div>
</body>
</html>
```
