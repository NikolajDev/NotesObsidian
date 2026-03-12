# CSS Comments

## Description
Comments are ignored by the browser. Used to explain code or temporarily disable rules.

## Syntax
```css
/* This is a CSS comment */

p {
  color: red; /* inline comment */
  /* font-size: 16px; — this line is disabled */
}
```

## Example
```css
/* ========================
   Typography
   ======================== */
h1 {
  font-size: 2rem;
  color: #222;
}

/* TODO: add mobile styles */
p {
  line-height: 1.6;
  /* color: blue; */ /* disabled temporarily */
  color: #444;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body>
  <h1 style="font-size: 2rem; color: #222;">This heading has styles applied</h1>
  <p style="line-height: 1.6; color: #444;">Comments in CSS are invisible — they only help developers read the code.</p>
</body>
</html>
```

## Notes
- CSS only supports `/* */` comments — no `//` single-line comments
- Use comments to organize sections in large CSS files
