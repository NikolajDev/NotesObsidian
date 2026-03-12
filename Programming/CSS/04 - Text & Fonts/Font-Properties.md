# Font Properties

## Properties

| Property | Purpose |
|----------|---------|
| `font-family` | Font name / stack |
| `font-size` | Text size |
| `font-weight` | Bold / thin |
| `font-style` | Normal / italic |
| `font-variant` | Small caps etc. |
| `font` | Shorthand |

## Example
```css
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size: 16px;
  font-weight: 400;
  font-style: normal;
}

h1 {
  font-size: 2.5rem;
  font-weight: 700;
  font-family: Georgia, serif;
}

.subtitle {
  font-size: 1.2rem;
  font-weight: 300;
  font-style: italic;
}

/* Shorthand: style weight size/line-height family */
p {
  font: italic 400 16px/1.6 Arial, sans-serif;
}
```

## Font Size Units

| Unit | Description |
|------|-------------|
| `px` | Fixed pixels |
| `rem` | Relative to root font size |
| `em` | Relative to parent font size |
| `%` | Relative to parent |
| `vw` | Relative to viewport width |

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="padding: 20px; background: #fafafa;">
  <p style="font-family: Georgia, serif; font-size: 2rem; font-weight: 700;">Georgia, Bold, 2rem</p>
  <p style="font-family: Arial, sans-serif; font-size: 1rem; font-weight: 400;">Arial, Normal, 1rem</p>
  <p style="font-family: 'Courier New', monospace; font-size: 1rem; font-style: italic;">Courier New, Italic</p>
  <p style="font-family: Arial; font-size: 1.2rem; font-weight: 300;">Arial, Light (300)</p>
  <p style="font-family: Arial; font-size: 1.2rem; font-weight: 900;">Arial, Black (900)</p>
</body>
</html>
```
