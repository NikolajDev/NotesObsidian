# Viewport Units

## Units

| Unit | Description |
|------|-------------|
| `vw` | 1% of viewport width |
| `vh` | 1% of viewport height |
| `vmin` | 1% of smaller dimension |
| `vmax` | 1% of larger dimension |
| `svh` | Small viewport height (mobile-safe) |
| `dvh` | Dynamic viewport height |

## Example
```css
/* Full screen hero section */
.hero {
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* Responsive font size */
h1 {
  font-size: clamp(1.5rem, 4vw, 3rem);
  /* min: 1.5rem, preferred: 4vw, max: 3rem */
}

/* Full height sidebar */
.sidebar {
  height: 100vh;
  overflow-y: auto;
  position: sticky;
  top: 0;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 15px;">
  <div style="width: 50vw; background: #3498db; color: white; padding: 15px; border-radius: 4px;">width: 50vw (50% of window)</div>
  <div style="width: 75vw; background: #e74c3c; color: white; padding: 15px; border-radius: 4px;">width: 75vw (75% of window)</div>
  <p style="font-size: clamp(1rem, 3vw, 2.5rem); background: #2ecc71; color: white; padding: 15px; border-radius: 4px; margin: 0;">
    font-size: clamp(1rem, 3vw, 2.5rem) — resize window!
  </p>
</body>
</html>
```
