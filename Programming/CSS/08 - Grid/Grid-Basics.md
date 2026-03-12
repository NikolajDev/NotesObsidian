# CSS Grid – Basics

## Description
A two-dimensional layout system for rows AND columns simultaneously.

## Enabling Grid
```css
.container {
  display: grid;
}
```

## Basic Setup
```css
.container {
  display: grid;
  grid-template-columns: 200px 200px 200px;  /* 3 columns */
  grid-template-rows: 100px 100px;            /* 2 rows */
  gap: 16px;
}
```

## Useful Functions

```css
/* repeat() */
grid-template-columns: repeat(3, 1fr);   /* 3 equal columns */
grid-template-columns: repeat(4, 200px); /* 4 fixed columns */

/* fr unit — fraction of available space */
grid-template-columns: 1fr 2fr 1fr;  /* 25% 50% 25% */

/* minmax() */
grid-template-columns: repeat(3, minmax(150px, 1fr));

/* auto-fill / auto-fit (responsive) */
grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 20px;">
  <p style="margin:0;"><strong>repeat(3, 1fr)</strong></p>
  <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 10px;">
    <div style="background: #3498db; color: white; padding: 20px; border-radius: 4px; text-align: center;">1</div>
    <div style="background: #3498db; color: white; padding: 20px; border-radius: 4px; text-align: center;">2</div>
    <div style="background: #3498db; color: white; padding: 20px; border-radius: 4px; text-align: center;">3</div>
    <div style="background: #3498db; color: white; padding: 20px; border-radius: 4px; text-align: center;">4</div>
    <div style="background: #3498db; color: white; padding: 20px; border-radius: 4px; text-align: center;">5</div>
    <div style="background: #3498db; color: white; padding: 20px; border-radius: 4px; text-align: center;">6</div>
  </div>

  <p style="margin:0;"><strong>1fr 2fr 1fr</strong></p>
  <div style="display: grid; grid-template-columns: 1fr 2fr 1fr; gap: 10px;">
    <div style="background: #e74c3c; color: white; padding: 20px; border-radius: 4px; text-align: center;">1fr</div>
    <div style="background: #c0392b; color: white; padding: 20px; border-radius: 4px; text-align: center;">2fr</div>
    <div style="background: #e74c3c; color: white; padding: 20px; border-radius: 4px; text-align: center;">1fr</div>
  </div>
</body>
</html>
```
