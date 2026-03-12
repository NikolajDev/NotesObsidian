# Position Property

## Values

| Value | Description |
|-------|-------------|
| `static` | Default, normal flow |
| `relative` | Offset from its normal position |
| `absolute` | Positioned relative to nearest positioned ancestor |
| `fixed` | Fixed to the viewport (stays on scroll) |
| `sticky` | Relative until scroll threshold, then fixed |

## Example
```css
/* Relative — offset from normal position */
.shifted {
  position: relative;
  top: 10px;
  left: 20px;
}

/* Absolute — relative to positioned parent */
.parent {
  position: relative;
}
.child {
  position: absolute;
  top: 0;
  right: 0;
}

/* Fixed — sticks to screen */
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background: white;
  z-index: 100;
}

/* Sticky — sticks when scrolled to */
.header {
  position: sticky;
  top: 0;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <div style="position: relative; background: #ecf0f1; height: 120px; margin-bottom: 15px; border: 2px dashed #bdc3c7;">
    <p style="margin: 10px;">Parent (position: relative)</p>
    <div style="position: absolute; top: 10px; right: 10px; background: #e74c3c; color: white; padding: 6px 10px; border-radius: 4px;">absolute: top-right</div>
    <div style="position: absolute; bottom: 10px; left: 10px; background: #3498db; color: white; padding: 6px 10px; border-radius: 4px;">absolute: bottom-left</div>
  </div>
  <div style="position: relative; top: 20px; left: 30px; background: #2ecc71; color: white; padding: 10px; display: inline-block; border-radius: 4px;">relative: shifted 20px down, 30px right</div>
</body>
</html>
```
