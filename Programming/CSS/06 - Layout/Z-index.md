# Z-index

## Description
Controls the stacking order of overlapping elements.
Higher z-index = on top. Only works on positioned elements (not `static`).

## Example
```css
.box-1 {
  position: absolute;
  z-index: 1;
  background: #3498db;
}

.box-2 {
  position: absolute;
  z-index: 2; /* on top of box-1 */
  background: #e74c3c;
}

/* Modal overlay pattern */
.overlay {
  position: fixed;
  z-index: 100;
  inset: 0;
  background: rgba(0,0,0,0.5);
}

.modal {
  position: fixed;
  z-index: 101; /* above overlay */
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <div style="position: relative; height: 120px;">
    <div style="position: absolute; top: 0; left: 0; width: 100px; height: 100px; background: #3498db; color: white; z-index: 1; border-radius: 4px; display: flex; align-items: center; justify-content: center;">z-index: 1</div>
    <div style="position: absolute; top: 20px; left: 40px; width: 100px; height: 100px; background: #e74c3c; color: white; z-index: 3; border-radius: 4px; display: flex; align-items: center; justify-content: center;">z-index: 3</div>
    <div style="position: absolute; top: 40px; left: 80px; width: 100px; height: 100px; background: #2ecc71; color: white; z-index: 2; border-radius: 4px; display: flex; align-items: center; justify-content: center;">z-index: 2</div>
  </div>
</body>
</html>
```

## Notes
- Requires `position` other than `static`
- Avoid very high values (999, 9999) — creates maintenance issues
- Common pattern: overlays at 100, modals at 200, tooltips at 300
