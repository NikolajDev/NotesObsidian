# CSS Backgrounds

## Properties

| Property | Purpose |
|----------|---------|
| `background-color` | Solid background color |
| `background-image` | Image as background |
| `background-repeat` | How image repeats |
| `background-size` | Image size |
| `background-position` | Image position |
| `background-attachment` | Scroll or fixed |

## Example
```css
/* Solid color */
body {
  background-color: #f5f5f5;
}

/* Image */
.hero {
  background-image: url('hero.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  height: 400px;
}

/* Shorthand */
.banner {
  background: #333 url('pattern.png') center/cover no-repeat;
}

/* Multiple backgrounds */
.layered {
  background:
    url('overlay.png') center/cover,
    url('texture.jpg') repeat;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 15px;">
  <div style="background-color: #3498db; color: white; padding: 20px; border-radius: 4px;">background-color: #3498db</div>
  <div style="background: linear-gradient(135deg, #667eea, #764ba2); color: white; padding: 20px; border-radius: 4px; height: 80px; display: flex; align-items: center;">background: gradient (see Gradients note)</div>
  <div style="background-color: #2ecc71; background-image: repeating-linear-gradient(45deg, transparent, transparent 10px, rgba(255,255,255,0.1) 10px, rgba(255,255,255,0.1) 20px); color: white; padding: 20px; border-radius: 4px;">background-color + background-image pattern</div>
</body>
</html>
```
