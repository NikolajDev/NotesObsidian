# CSS Gradients

## Types

| Type | Description |
|------|-------------|
| `linear-gradient` | Left to right, top to bottom, any angle |
| `radial-gradient` | Radiates from center outward |
| `conic-gradient` | Rotates around a center point |

## Linear Gradient
```css
/* Basic */
background: linear-gradient(red, blue);

/* With angle */
background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
background: linear-gradient(to right, #f7971e, #ffd200);

/* Multiple stops */
background: linear-gradient(to right, #e74c3c, #f39c12, #2ecc71);

/* With percentage stops */
background: linear-gradient(to right, #667eea 0%, #764ba2 100%);
```

## Radial Gradient
```css
background: radial-gradient(circle, #ff6b6b, #4ecdc4);
background: radial-gradient(ellipse at top, #3498db, #2c3e50);
```

## Conic Gradient
```css
/* Color wheel */
background: conic-gradient(red, yellow, green, blue, red);

/* Pie chart segments */
background: conic-gradient(#e74c3c 0% 30%, #3498db 30% 70%, #2ecc71 70% 100%);
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 12px;">
  <div style="background: linear-gradient(to right, #e74c3c, #f39c12); color: white; padding: 20px; border-radius: 6px;">linear-gradient(to right, red → orange)</div>
  <div style="background: linear-gradient(135deg, #667eea, #764ba2); color: white; padding: 20px; border-radius: 6px;">linear-gradient(135deg, purple tones)</div>
  <div style="background: radial-gradient(circle, #f9ca24, #f0932b); color: white; padding: 20px; border-radius: 6px;">radial-gradient(circle, yellow → orange)</div>
  <div style="background: conic-gradient(#e74c3c 0% 30%, #3498db 30% 70%, #2ecc71 70% 100%); width: 100px; height: 100px; border-radius: 50%; align-self: flex-start;"></div>
  <p style="margin: 0; color: #555; font-size: 0.9em;">↑ conic-gradient pie chart</p>
</body>
</html>
```
