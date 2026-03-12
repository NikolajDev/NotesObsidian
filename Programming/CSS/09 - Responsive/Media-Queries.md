# Media Queries

## Description
Apply CSS only when certain conditions are met (screen size, orientation, etc.).

## Syntax
```css
@media (condition) {
  /* CSS rules */
}
```

## Common Breakpoints
```css
/* Mobile first approach */
/* Base styles: mobile */
.container { padding: 16px; }

/* Tablet */
@media (min-width: 768px) {
  .container { padding: 24px; }
  .grid { display: grid; grid-template-columns: repeat(2, 1fr); }
}

/* Desktop */
@media (min-width: 1024px) {
  .container { max-width: 1200px; margin: 0 auto; }
  .grid { grid-template-columns: repeat(3, 1fr); }
}

/* Large Desktop */
@media (min-width: 1440px) {
  .grid { grid-template-columns: repeat(4, 1fr); }
}
```

## Other Conditions
```css
/* Dark mode */
@media (prefers-color-scheme: dark) {
  body { background: #1a1a1a; color: white; }
}

/* Orientation */
@media (orientation: landscape) {
  .hero { height: 50vh; }
}

/* Print */
@media print {
  .no-print { display: none; }
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    .responsive-box {
      background: #e74c3c;
      color: white;
      padding: 20px;
      border-radius: 4px;
      text-align: center;
    }
    @media (min-width: 600px) {
      .responsive-box { background: #3498db; }
    }
    @media (min-width: 900px) {
      .responsive-box { background: #2ecc71; }
    }
  </style>
</head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <div class="responsive-box">
    Resize the window!<br>
    Red = mobile | Blue = tablet | Green = desktop
  </div>
</body>
</html>
```
