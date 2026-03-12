# Border

## Properties

| Property | Purpose |
|----------|---------|
| `border-width` | Thickness |
| `border-style` | solid, dashed, dotted, double... |
| `border-color` | Color |
| `border` | Shorthand |
| `border-radius` | Rounded corners |
| `outline` | Like border but outside box model |

## Example
```css
/* Shorthand */
.box {
  border: 2px solid #333;
}

/* Individual sides */
.underline {
  border-top: none;
  border-right: none;
  border-bottom: 2px solid #3498db;
  border-left: none;
}

/* Border styles */
.dashed  { border: 2px dashed #e74c3c; }
.dotted  { border: 2px dotted #2ecc71; }
.double  { border: 4px double #9b59b6; }

/* Rounded corners */
.rounded { border-radius: 8px; }
.pill    { border-radius: 50px; }
.circle  { border-radius: 50%; }

/* Individual corners */
.custom {
  border-radius: 10px 0 10px 0;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-wrap: wrap; gap: 15px;">
  <div style="border: 2px solid #333; padding: 12px 20px;">solid</div>
  <div style="border: 2px dashed #e74c3c; padding: 12px 20px;">dashed</div>
  <div style="border: 2px dotted #2ecc71; padding: 12px 20px;">dotted</div>
  <div style="border: 4px double #9b59b6; padding: 12px 20px;">double</div>
  <div style="border: 2px solid #3498db; border-radius: 8px; padding: 12px 20px;">rounded</div>
  <div style="border: 2px solid #e67e22; border-radius: 50px; padding: 12px 20px;">pill</div>
  <div style="border: 2px solid #1abc9c; border-radius: 50%; width: 60px; height: 60px; display: flex; align-items: center; justify-content: center;">circle</div>
  <div style="border-bottom: 3px solid #3498db; padding: 12px 20px;">bottom only</div>
</body>
</html>
```
