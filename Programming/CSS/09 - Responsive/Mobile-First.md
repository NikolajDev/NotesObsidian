# Mobile First Design

## Description
Design for mobile screens first, then add complexity for larger screens using `min-width` media queries.

## Mobile First vs Desktop First

```css
/* ❌ Desktop First (add overrides for smaller screens) */
.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
@media (max-width: 768px) {
  .grid { grid-template-columns: 1fr; }
}

/* ✅ Mobile First (start simple, enhance upward) */
.grid {
  display: grid;
  grid-template-columns: 1fr;
}
@media (min-width: 768px) {
  .grid { grid-template-columns: repeat(2, 1fr); }
}
@media (min-width: 1024px) {
  .grid { grid-template-columns: repeat(3, 1fr); }
}
```

## Common Mobile First Pattern
```css
/* Base (mobile) */
.navbar {
  display: flex;
  flex-direction: column;
  padding: 16px;
}

.nav-links {
  display: none; /* hidden on mobile */
}

.hamburger {
  display: block;
}

/* Tablet */
@media (min-width: 768px) {
  .navbar {
    flex-direction: row;
    align-items: center;
  }
  .nav-links { display: flex; gap: 20px; }
  .hamburger { display: none; }
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    .mf-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 10px;
    }
    @media (min-width: 600px) {
      .mf-grid { grid-template-columns: repeat(2, 1fr); }
    }
    @media (min-width: 900px) {
      .mf-grid { grid-template-columns: repeat(3, 1fr); }
    }
  </style>
</head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <p>Resize window to see mobile-first grid adapt:</p>
  <div class="mf-grid">
    <div style="background: #3498db; color: white; padding: 20px; border-radius: 4px; text-align: center;">Card 1</div>
    <div style="background: #3498db; color: white; padding: 20px; border-radius: 4px; text-align: center;">Card 2</div>
    <div style="background: #3498db; color: white; padding: 20px; border-radius: 4px; text-align: center;">Card 3</div>
  </div>
</body>
</html>
```
