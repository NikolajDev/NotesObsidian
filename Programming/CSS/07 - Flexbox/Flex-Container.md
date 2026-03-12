# Flex Container Properties

## Properties (on parent)

| Property | Values | Purpose |
|----------|--------|---------|
| `flex-direction` | row, column, row-reverse, column-reverse | Direction of items |
| `justify-content` | flex-start, center, flex-end, space-between, space-around, space-evenly | Main axis alignment |
| `align-items` | stretch, center, flex-start, flex-end, baseline | Cross axis alignment |
| `flex-wrap` | nowrap, wrap, wrap-reverse | Allow wrapping |
| `gap` | px, rem | Space between items |
| `align-content` | same as justify-content | Multi-line cross axis |

## Example
```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 16px;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 15px;">

  <p style="margin:0;"><strong>justify-content: space-between</strong></p>
  <div style="display: flex; justify-content: space-between; background: #ecf0f1; padding: 10px; border-radius: 4px;">
    <div style="background: #3498db; color: white; padding: 10px 16px; border-radius: 4px;">A</div>
    <div style="background: #3498db; color: white; padding: 10px 16px; border-radius: 4px;">B</div>
    <div style="background: #3498db; color: white; padding: 10px 16px; border-radius: 4px;">C</div>
  </div>

  <p style="margin:0;"><strong>justify-content: space-evenly + align-items: center</strong></p>
  <div style="display: flex; justify-content: space-evenly; align-items: center; background: #ecf0f1; padding: 10px; border-radius: 4px; height: 80px;">
    <div style="background: #e74c3c; color: white; padding: 6px 16px; border-radius: 4px;">Short</div>
    <div style="background: #e74c3c; color: white; padding: 16px; border-radius: 4px;">Tall</div>
    <div style="background: #e74c3c; color: white; padding: 6px 16px; border-radius: 4px;">Short</div>
  </div>

  <p style="margin:0;"><strong>flex-wrap: wrap + gap</strong></p>
  <div style="display: flex; flex-wrap: wrap; gap: 10px; background: #ecf0f1; padding: 10px; border-radius: 4px;">
    <div style="background: #2ecc71; color: white; padding: 10px 20px; border-radius: 4px;">Item 1</div>
    <div style="background: #2ecc71; color: white; padding: 10px 20px; border-radius: 4px;">Item 2</div>
    <div style="background: #2ecc71; color: white; padding: 10px 20px; border-radius: 4px;">Item 3</div>
    <div style="background: #2ecc71; color: white; padding: 10px 20px; border-radius: 4px;">Item 4</div>
    <div style="background: #2ecc71; color: white; padding: 10px 20px; border-radius: 4px;">Item 5</div>
  </div>
</body>
</html>
```
