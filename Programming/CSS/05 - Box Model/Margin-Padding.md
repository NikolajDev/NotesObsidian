# Margin & Padding

## Description

| Property | Space |
|----------|-------|
| `margin` | Outside the border (pushes away other elements) |
| `padding` | Inside the border (pushes content away from border) |

## Syntax
```css
/* All sides */
margin: 20px;
padding: 20px;

/* Top/Bottom  Left/Right */
margin: 10px 20px;

/* Top  Right  Bottom  Left (clockwise) */
margin: 10px 20px 10px 20px;
padding: 5px 10px 15px 20px;

/* Individual sides */
margin-top: 10px;
margin-right: 20px;
margin-bottom: 10px;
margin-left: 20px;

padding-top: 5px;
padding-right: 10px;
padding-bottom: 15px;
padding-left: 20px;
```

## Common Tricks
```css
/* Center a block element horizontally */
.container {
  width: 800px;
  margin: 0 auto;
}

/* Remove default browser margin/padding */
* {
  margin: 0;
  padding: 0;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; background: #f0f0f0;">
  <div style="background: #3498db; color: white; padding: 30px; margin: 20px; border-radius: 4px; text-align: center;">
    padding: 30px — large inner space
  </div>
  <div style="background: #e74c3c; color: white; padding: 5px; margin: 40px; border-radius: 4px; text-align: center;">
    padding: 5px + margin: 40px — tight content, far from others
  </div>
  <div style="background: #2ecc71; color: white; padding: 15px 40px; margin: 10px auto; width: 300px; border-radius: 4px; text-align: center;">
    margin: 0 auto — centered block
  </div>
</body>
</html>
```
