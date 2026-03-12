# CSS Syntax

## Structure
```css
selector {
  property: value;
}
```

## Full Example
```css
/* Single property */
h1 {
  color: red;
}

/* Multiple properties */
p {
  color: #333333;
  font-size: 16px;
  line-height: 1.5;
  margin-bottom: 10px;
}

/* Multiple selectors, same rules */
h1, h2, h3 {
  font-family: Arial, sans-serif;
  color: navy;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body>
  <h1 style="color: red;">Red Heading</h1>
  <p style="color: #333333; font-size: 16px; line-height: 1.5; margin-bottom: 10px;">
    This paragraph uses multiple CSS properties at once.
  </p>
  <h2 style="font-family: Arial, sans-serif; color: navy;">Navy Subtitle</h2>
  <h3 style="font-family: Arial, sans-serif; color: navy;">Also Navy</h3>
</body>
</html>
```

## Notes
- Each declaration ends with a semicolon `;`
- Rules are wrapped in curly braces `{}`
- CSS is case-insensitive but convention is lowercase
