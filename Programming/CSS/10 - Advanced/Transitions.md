# CSS Transitions

## Description
Smoothly animate changes between CSS property values.

## Syntax
```css
element {
  transition: property duration timing-function delay;
}
```

## Example
```css
/* Single property */
.button {
  background-color: #3498db;
  transition: background-color 0.3s ease;
}
.button:hover {
  background-color: #2980b9;
}

/* Multiple properties */
.card {
  transform: translateY(0);
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  transition:
    transform 0.3s ease,
    box-shadow 0.3s ease;
}
.card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0,0,0,0.15);
}

/* All properties */
.element {
  transition: all 0.3s ease;
}
```

## Timing Functions
```css
transition-timing-function: ease;        /* default */
transition-timing-function: linear;      /* constant speed */
transition-timing-function: ease-in;     /* slow start */
transition-timing-function: ease-out;    /* slow end */
transition-timing-function: ease-in-out; /* slow start and end */
transition-timing-function: cubic-bezier(0.68, -0.55, 0.27, 1.55); /* custom */
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    .t-btn {
      background: #3498db; color: white; padding: 12px 24px;
      border: none; border-radius: 6px; cursor: pointer; font-size: 1rem;
      transition: background 0.3s ease, transform 0.2s ease;
    }
    .t-btn:hover { background: #e74c3c; transform: scale(1.05); }
    .t-card {
      background: white; padding: 20px; border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1); cursor: pointer;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .t-card:hover { transform: translateY(-6px); box-shadow: 0 12px 24px rgba(0,0,0,0.15); }
  </style>
</head>
<body style="font-family: Arial, sans-serif; padding: 20px; background: #f5f5f5; display: flex; flex-direction: column; gap: 20px; align-items: flex-start;">
  <button class="t-btn">Hover me — color + scale</button>
  <div class="t-card" style="width: 200px;">Hover me — lift card effect</div>
</body>
</html>
```
