# Grid Template – Placing Items

## Placing Items

```css
.item {
  grid-column: 1 / 3;    /* from line 1 to line 3 (spans 2 cols) */
  grid-row: 1 / 2;       /* row 1 */
}

/* Shorthand */
.item {
  grid-column: span 2;   /* span 2 columns */
  grid-row: span 3;      /* span 3 rows */
}
```

## Full Example
```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: auto;
  gap: 12px;
}

.header {
  grid-column: 1 / -1;  /* span all columns (-1 = last line) */
}

.sidebar {
  grid-column: 1 / 2;
  grid-row: 2 / 4;       /* span 2 rows */
}

.main {
  grid-column: 2 / -1;
}

.footer {
  grid-column: 1 / -1;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 10px;">
    <div style="grid-column: 1 / -1; background: #2c3e50; color: white; padding: 15px; border-radius: 4px; text-align: center;">Header (1 / -1)</div>
    <div style="grid-column: 1 / 2; grid-row: 2 / 4; background: #8e44ad; color: white; padding: 15px; border-radius: 4px; text-align: center;">Sidebar<br>row 2/4</div>
    <div style="grid-column: 2 / -1; background: #3498db; color: white; padding: 15px; border-radius: 4px; text-align: center;">Main Content (2 / -1)</div>
    <div style="grid-column: 2 / -1; background: #2980b9; color: white; padding: 15px; border-radius: 4px; text-align: center;">Second row main</div>
    <div style="grid-column: 1 / -1; background: #7f8c8d; color: white; padding: 15px; border-radius: 4px; text-align: center;">Footer (1 / -1)</div>
  </div>
</body>
</html>
```
