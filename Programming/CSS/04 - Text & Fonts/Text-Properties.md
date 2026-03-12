# Text Properties

## Properties

| Property | Purpose |
|----------|---------|
| `color` | Text color |
| `text-align` | Alignment |
| `text-decoration` | Underline, line-through etc. |
| `text-transform` | Uppercase, lowercase, capitalize |
| `letter-spacing` | Space between characters |
| `word-spacing` | Space between words |
| `line-height` | Space between lines |
| `text-shadow` | Shadow behind text |
| `text-indent` | First line indent |
| `white-space` | Wrapping behavior |
| `overflow` | Handle overflow text |
| `text-overflow` | Ellipsis for overflow |

## Example
```css
h1 {
  text-align: center;
  text-transform: uppercase;
  letter-spacing: 4px;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
}

p {
  line-height: 1.8;
  text-indent: 2em;
  color: #444;
}

.badge {
  text-transform: uppercase;
  letter-spacing: 2px;
  font-size: 0.75rem;
}

/* Truncate with ellipsis */
.truncate {
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  max-width: 200px;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 12px;">
  <h1 style="text-align: center; text-transform: uppercase; letter-spacing: 4px; text-shadow: 2px 2px 4px rgba(0,0,0,0.2); color: #2c3e50;">Styled Heading</h1>
  <p style="line-height: 1.8; text-indent: 2em; color: #444;">This paragraph has a text indent on the first line and generous line height for better readability.</p>
  <p style="text-decoration: line-through; color: #e74c3c;">Strikethrough text</p>
  <p style="text-decoration: underline wavy #3498db;">Wavy underline</p>
  <div style="white-space: nowrap; overflow: hidden; text-overflow: ellipsis; max-width: 200px; border: 1px solid #ddd; padding: 6px;">Very long text that gets truncated with ellipsis</div>
</body>
</html>
```
