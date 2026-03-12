# CSS Transforms

## Description
Move, rotate, scale, or skew elements without affecting document flow.

## 2D Transform Functions

| Function | Description |
|----------|-------------|
| `translate(x, y)` | Move element |
| `rotate(deg)` | Rotate element |
| `scale(x, y)` | Resize element |
| `skew(x, y)` | Skew element |
| `matrix(...)` | All in one (advanced) |

## Example
```css
/* Move */
.moved {
  transform: translate(50px, 20px);
}

/* Rotate */
.rotated {
  transform: rotate(45deg);
}

/* Scale */
.scaled {
  transform: scale(1.5);          /* uniform */
  transform: scale(2, 0.5);       /* x=2, y=0.5 */
}

/* Skew */
.skewed {
  transform: skew(15deg, 5deg);
}

/* Combine multiple */
.combined {
  transform: translate(20px, 10px) rotate(10deg) scale(1.1);
}

/* Center element absolutely — classic trick */
.centered {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

## 3D Transforms
```css
.card {
  transform: perspective(500px) rotateY(20deg);
}

.flip:hover {
  transform: rotateY(180deg);
  transition: transform 0.6s ease;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 40px; display: flex; flex-wrap: wrap; gap: 30px; align-items: center;">
  <div style="background: #3498db; color: white; padding: 14px 20px; border-radius: 4px; transform: translate(0px, 0px);">translate(0)</div>
  <div style="background: #e74c3c; color: white; padding: 14px 20px; border-radius: 4px; transform: rotate(15deg);">rotate(15deg)</div>
  <div style="background: #2ecc71; color: white; padding: 14px 20px; border-radius: 4px; transform: scale(1.3);">scale(1.3)</div>
  <div style="background: #9b59b6; color: white; padding: 14px 20px; border-radius: 4px; transform: skew(10deg);">skew(10deg)</div>
  <div style="background: #e67e22; color: white; padding: 14px 20px; border-radius: 4px; transform: rotate(-10deg) scale(1.1) translateX(10px);">combined</div>
</body>
</html>
```
