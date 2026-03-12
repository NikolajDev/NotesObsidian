# Pseudo-Classes

## Description
Target elements based on their **state** or **position**.
Written with a single colon `:`.

## Common Pseudo-Classes

| Pseudo-class | Targets |
|--------------|---------|
| `:hover` | Element being hovered |
| `:focus` | Focused input/element |
| `:active` | Element being clicked |
| `:visited` | Visited link |
| `:first-child` | First child element |
| `:last-child` | Last child element |
| `:nth-child(n)` | nth child element |
| `:not(selector)` | Elements that don't match |

## Example
```css
/* Hover effect */
a:hover {
  color: red;
  text-decoration: underline;
}

/* Focus on input */
input:focus {
  border-color: blue;
  outline: none;
  box-shadow: 0 0 5px rgba(0,0,255,0.3);
}

/* First and last child */
li:first-child {
  font-weight: bold;
}

li:last-child {
  color: gray;
}

/* Every even row */
tr:nth-child(even) {
  background-color: #f2f2f2;
}

/* Not a specific class */
p:not(.special) {
  color: #555;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    .demo-link:hover { color: red; }
    .demo-input:focus { border-color: blue; outline: none; box-shadow: 0 0 5px rgba(0,0,255,0.3); }
    .demo-list li:first-child { font-weight: bold; }
    .demo-list li:last-child { color: gray; }
  </style>
</head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <a href="#" class="demo-link" style="color: coral;">Hover over me</a><br><br>
  <input class="demo-input" type="text" placeholder="Click to focus me" style="padding: 6px; border: 2px solid #ccc;"><br><br>
  <ul class="demo-list" style="padding-left: 20px;">
    <li>First item (bold)</li>
    <li>Middle item</li>
    <li>Last item (gray)</li>
  </ul>
</body>
</html>
```
