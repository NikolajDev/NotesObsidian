# CSS Colors

## Description
CSS supports multiple formats for defining colors.

## Color Formats

```css
/* Named colors */
color: red;
color: coral;
color: steelblue;

/* Hex */
color: #ff0000;        /* red */
color: #333;           /* short hex = #333333 */

/* RGB */
color: rgb(255, 0, 0);       /* red */
color: rgb(51, 51, 51);      /* dark gray */

/* RGBA (with transparency) */
color: rgba(255, 0, 0, 0.5); /* 50% transparent red */

/* HSL */
color: hsl(0, 100%, 50%);    /* red */
color: hsl(210, 70%, 50%);   /* blue */

/* HSLA */
color: hsla(0, 100%, 50%, 0.3);
```

## Common Properties
```css
p {
  color: #333;                        /* text color */
  background-color: #f0f0f0;          /* background */
  border: 2px solid rgba(0,0,0,0.2);  /* border color */
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 10px;">
  <div style="background-color: #e74c3c; color: white; padding: 10px; border-radius: 4px;">Hex: #e74c3c</div>
  <div style="background-color: rgb(52, 152, 219); color: white; padding: 10px; border-radius: 4px;">RGB: rgb(52, 152, 219)</div>
  <div style="background-color: rgba(46, 204, 113, 0.7); color: white; padding: 10px; border-radius: 4px;">RGBA: 70% opacity green</div>
  <div style="background-color: hsl(270, 60%, 50%); color: white; padding: 10px; border-radius: 4px;">HSL: hsl(270, 60%, 50%)</div>
  <div style="background-color: coral; color: white; padding: 10px; border-radius: 4px;">Named: coral</div>
</body>
</html>
```
