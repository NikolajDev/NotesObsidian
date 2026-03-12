# What is CSS?

## Description
CSS (Cascading Style Sheets) describes how HTML elements should look.
Without CSS, web pages are plain black text on white background.

## CSS Rule Structure
```css
selector {
  property: value;
  property: value;
}
```

## Example
```css
h1 {
  color: blue;
  font-size: 32px;
  text-align: center;
}

p {
  color: #333;
  line-height: 1.6;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body>
  <h1 style="color: blue; font-size: 32px; text-align: center;">Hello CSS!</h1>
  <p style="color: #333; line-height: 1.6;">This paragraph has custom color and line height applied via CSS.</p>
  <p style="color: #333; line-height: 1.6;">Without CSS, both paragraphs would look identical and plain.</p>
</body>
</html>
```

## Notes
- CSS stands for **C**ascading **S**tyle **S**heets
- "Cascading" means styles flow down and override each other by rules
- One CSS file can style an entire website
