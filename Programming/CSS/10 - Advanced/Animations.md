# CSS Animations

## Description
Create complex multi-step animations using `@keyframes`.

## Syntax
```css
/* 1. Define the animation */
@keyframes animation-name {
  from { /* start state */ }
  to   { /* end state */ }
}

/* Or with percentages */
@keyframes animation-name {
  0%   { /* start */ }
  50%  { /* middle */ }
  100% { /* end */ }
}

/* 2. Apply to element */
.element {
  animation: animation-name duration timing-function delay iteration-count direction;
}
```

## Example
```css
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to   { opacity: 1; transform: translateY(0); }
}

@keyframes pulse {
  0%, 100% { transform: scale(1); }
  50%       { transform: scale(1.05); }
}

@keyframes spin {
  from { transform: rotate(0deg); }
  to   { transform: rotate(360deg); }
}

.fade-in {
  animation: fadeIn 0.5s ease forwards;
}

.pulse {
  animation: pulse 2s ease-in-out infinite;
}

.spinner {
  animation: spin 1s linear infinite;
}
```

## Properties
```css
.element {
  animation-name: fadeIn;
  animation-duration: 0.5s;
  animation-timing-function: ease;
  animation-delay: 0.2s;
  animation-iteration-count: 1;      /* or infinite */
  animation-direction: normal;       /* or reverse, alternate */
  animation-fill-mode: forwards;     /* keep end state */
  animation-play-state: running;     /* or paused */
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    @keyframes fadeSlideIn { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }
    @keyframes pulse { 0%,100% { transform: scale(1); } 50% { transform: scale(1.08); } }
    @keyframes spin { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }
    @keyframes colorShift { 0% { background: #3498db; } 33% { background: #e74c3c; } 66% { background: #2ecc71; } 100% { background: #3498db; } }
    .anim-fade { animation: fadeSlideIn 1s ease forwards; background: #3498db; color: white; padding: 12px 20px; border-radius: 6px; display: inline-block; }
    .anim-pulse { animation: pulse 2s ease-in-out infinite; background: #e74c3c; color: white; padding: 12px 20px; border-radius: 6px; display: inline-block; }
    .anim-spin { animation: spin 1.5s linear infinite; width: 40px; height: 40px; border: 4px solid #f0f0f0; border-top-color: #3498db; border-radius: 50%; }
    .anim-color { animation: colorShift 3s ease infinite; color: white; padding: 12px 20px; border-radius: 6px; display: inline-block; }
  </style>
</head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 20px; align-items: flex-start;">
  <div class="anim-fade">fadeSlideIn</div>
  <div class="anim-pulse">pulse (infinite)</div>
  <div class="anim-spin"></div>
  <div class="anim-color">color shift (infinite)</div>
</body>
</html>
```
