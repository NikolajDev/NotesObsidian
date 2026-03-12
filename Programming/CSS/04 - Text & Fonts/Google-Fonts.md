# Google Fonts

## Description
Free web fonts from Google that you can use on any website.
Website: https://fonts.google.com

## How to Use

### 1. Import in HTML `<head>`
```html
<head>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&family=Playfair+Display:ital@1&display=swap" rel="stylesheet">
</head>
```

### 2. Import in CSS
```css
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');
```

### 3. Use in CSS
```css
body {
  font-family: 'Roboto', sans-serif;
}

h1 {
  font-family: 'Playfair Display', serif;
  font-style: italic;
}
```

## Popular Font Pairings
```css
/* Classic pairing */
h1, h2 { font-family: 'Playfair Display', serif; }
body    { font-family: 'Source Sans Pro', sans-serif; }

/* Modern pairing */
h1, h2 { font-family: 'Poppins', sans-serif; font-weight: 700; }
body    { font-family: 'Poppins', sans-serif; font-weight: 400; }

/* Techy */
h1, h2 { font-family: 'Space Grotesk', sans-serif; }
code    { font-family: 'JetBrains Mono', monospace; }
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital@0;1&family=Roboto:wght@300;400;700&family=JetBrains+Mono&display=swap" rel="stylesheet">
</head>
<body style="padding: 20px; background: #fafafa; display: flex; flex-direction: column; gap: 12px;">
  <h1 style="font-family: 'Playfair Display', serif; font-size: 2.5rem; color: #2c3e50;">Playfair Display – Elegant Serif</h1>
  <p style="font-family: 'Roboto', sans-serif; font-weight: 300; font-size: 1.1rem; color: #555;">Roboto Light – Clean and modern for body text.</p>
  <p style="font-family: 'Roboto', sans-serif; font-weight: 700; font-size: 1.1rem; color: #333;">Roboto Bold – Same font, different weight.</p>
  <code style="font-family: 'JetBrains Mono', monospace; background: #f0f0f0; padding: 8px 12px; border-radius: 4px;">JetBrains Mono – Perfect for code</code>
</body>
</html>
```

## Notes
- Use `display=swap` to prevent invisible text while font loads
- Limit to 2-3 fonts per page for performance
- `preconnect` hints speed up font loading
