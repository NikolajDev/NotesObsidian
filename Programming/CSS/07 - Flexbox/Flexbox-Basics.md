# Flexbox – Basics

## Description
A one-dimensional layout system for arranging items in a row or column.
Set on the **parent container**.

## Enabling Flexbox
```css
.container {
  display: flex;
}
```

## Main Axis vs Cross Axis
```
flex-direction: row (default)
→ Main axis: horizontal →
→ Cross axis: vertical ↓

flex-direction: column
→ Main axis: vertical ↓
→ Cross axis: horizontal →
```

## Quick Example
```css
.container {
  display: flex;
  flex-direction: row;        /* default */
  justify-content: center;    /* main axis */
  align-items: center;        /* cross axis */
  gap: 16px;
  height: 200px;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 15px;">
  <div style="display: flex; gap: 10px; background: #ecf0f1; padding: 10px; border-radius: 4px;">
    <div style="background: #3498db; color: white; padding: 12px 20px; border-radius: 4px;">Item 1</div>
    <div style="background: #e74c3c; color: white; padding: 12px 20px; border-radius: 4px;">Item 2</div>
    <div style="background: #2ecc71; color: white; padding: 12px 20px; border-radius: 4px;">Item 3</div>
  </div>
  <div style="display: flex; justify-content: center; gap: 10px; background: #ecf0f1; padding: 10px; border-radius: 4px;">
    <div style="background: #9b59b6; color: white; padding: 12px 20px; border-radius: 4px;">Centered</div>
    <div style="background: #9b59b6; color: white; padding: 12px 20px; border-radius: 4px;">Items</div>
  </div>
  <div style="display: flex; flex-direction: column; gap: 8px; background: #ecf0f1; padding: 10px; border-radius: 4px;">
    <div style="background: #e67e22; color: white; padding: 10px; border-radius: 4px;">Column</div>
    <div style="background: #e67e22; color: white; padding: 10px; border-radius: 4px;">Direction</div>
  </div>
</body>
</html>
```
