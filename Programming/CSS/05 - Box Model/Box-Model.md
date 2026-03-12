# The Box Model

## Description
Every HTML element is a rectangular box with 4 layers:

```
┌─────────────────────────────┐
│           MARGIN            │
│  ┌───────────────────────┐  │
│  │        BORDER         │  │
│  │  ┌─────────────────┐  │  │
│  │  │     PADDING     │  │  │
│  │  │  ┌───────────┐  │  │  │
│  │  │  │  CONTENT  │  │  │  │
│  │  │  └───────────┘  │  │  │
│  │  └─────────────────┘  │  │
│  └───────────────────────┘  │
└─────────────────────────────┘
```

## Example
```css
.box {
  /* Content */
  width: 200px;
  height: 100px;

  /* Padding – inside the border */
  padding: 20px;

  /* Border */
  border: 3px solid #333;

  /* Margin – outside the border */
  margin: 30px;

  background-color: lightblue;
}
```

## Total Size (default)
Total width = `width` + `padding-left` + `padding-right` + `border-left` + `border-right`

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; background: #f0f0f0;">
  <div style="margin: 30px; border: 3px solid #e74c3c; padding: 20px; width: 200px; background-color: #d5e8fa; font-size: 0.9em; text-align: center;">
    <span style="display: block; background: #aed6f1; padding: 10px;">
      content<br><small>200×auto</small>
    </span>
    <small style="color: #555;">padding: 20px</small>
  </div>
  <p style="color: #777; font-size: 0.85em;">Red = border, blue = padding, light blue = content, outer space = margin</p>
</body>
</html>
```
