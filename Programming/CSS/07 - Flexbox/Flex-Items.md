# Flex Item Properties

## Properties (on children)

| Property | Purpose |
|----------|---------|
| `flex-grow` | How much item grows relative to others |
| `flex-shrink` | How much item shrinks when needed |
| `flex-basis` | Initial size before growing/shrinking |
| `flex` | Shorthand: grow shrink basis |
| `align-self` | Override container's align-items |
| `order` | Change visual order |

## Example
```css
/* Equal width columns */
.item {
  flex: 1;  /* shorthand for flex: 1 1 0 */
}

/* One item takes double space */
.wide {
  flex: 2;
}

/* Fixed size item */
.sidebar {
  flex: 0 0 250px; /* don't grow, don't shrink, always 250px */
}

/* Override alignment */
.item-special {
  align-self: flex-end;
}

/* Change order */
.first {
  order: -1; /* appears first regardless of DOM order */
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 15px;">

  <p style="margin:0;"><strong>flex: 1 — equal columns</strong></p>
  <div style="display: flex; gap: 10px;">
    <div style="flex: 1; background: #3498db; color: white; padding: 12px; border-radius: 4px; text-align: center;">flex: 1</div>
    <div style="flex: 1; background: #3498db; color: white; padding: 12px; border-radius: 4px; text-align: center;">flex: 1</div>
    <div style="flex: 1; background: #3498db; color: white; padding: 12px; border-radius: 4px; text-align: center;">flex: 1</div>
  </div>

  <p style="margin:0;"><strong>flex: 2 takes double space</strong></p>
  <div style="display: flex; gap: 10px;">
    <div style="flex: 1; background: #9b59b6; color: white; padding: 12px; border-radius: 4px; text-align: center;">flex: 1</div>
    <div style="flex: 2; background: #8e44ad; color: white; padding: 12px; border-radius: 4px; text-align: center;">flex: 2 (double)</div>
    <div style="flex: 1; background: #9b59b6; color: white; padding: 12px; border-radius: 4px; text-align: center;">flex: 1</div>
  </div>

  <p style="margin:0;"><strong>align-self</strong></p>
  <div style="display: flex; gap: 10px; height: 80px; align-items: flex-start; background: #ecf0f1; padding: 10px; border-radius: 4px;">
    <div style="background: #e74c3c; color: white; padding: 10px; border-radius: 4px; align-self: flex-start;">top</div>
    <div style="background: #e74c3c; color: white; padding: 10px; border-radius: 4px; align-self: center;">center</div>
    <div style="background: #e74c3c; color: white; padding: 10px; border-radius: 4px; align-self: flex-end;">bottom</div>
  </div>
</body>
</html>
```
