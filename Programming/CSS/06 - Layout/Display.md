# Display Property

## Description
Controls how an element is rendered in the layout.

## Common Values

| Value | Description |
|-------|-------------|
| `block` | Full width, starts on new line |
| `inline` | Width = content, stays in line |
| `inline-block` | Inline but accepts width/height |
| `none` | Hidden, removed from layout |
| `flex` | Flexbox container |
| `grid` | Grid container |

## Example
```css
/* Block — takes full width */
div { display: block; }

/* Inline — stays in text flow */
span { display: inline; }

/* Inline-block — inline but accepts dimensions */
.badge {
  display: inline-block;
  width: 80px;
  height: 24px;
  text-align: center;
}

/* Hidden */
.hidden { display: none; }

/* Show on hover */
.tooltip { display: none; }
.parent:hover .tooltip { display: block; }
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px; display: flex; flex-direction: column; gap: 12px;">
  <div style="background: #3498db; color: white; padding: 10px;">display: block — full width</div>
  <div>
    <span style="background: #e74c3c; color: white; padding: 4px 8px;">inline</span>
    <span style="background: #e74c3c; color: white; padding: 4px 8px;">inline</span>
    <span style="background: #e74c3c; color: white; padding: 4px 8px;">stays in line</span>
  </div>
  <div>
    <span style="display: inline-block; background: #2ecc71; color: white; padding: 8px 16px; width: 120px; text-align: center; border-radius: 4px;">inline-block</span>
    <span style="display: inline-block; background: #9b59b6; color: white; padding: 8px 16px; width: 120px; text-align: center; border-radius: 4px;">inline-block</span>
  </div>
</body>
</html>
```
