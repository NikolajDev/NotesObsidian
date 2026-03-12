# Box Sizing

## Description
Controls how `width` and `height` are calculated.

## Values

| Value | Width includes |
|-------|---------------|
| `content-box` | Only content (default) |
| `border-box` | Content + padding + border |

## The Problem
```css
/* content-box (default) */
.box {
  width: 200px;
  padding: 20px;
  border: 2px solid;
  /* actual width = 200 + 40 + 4 = 244px ← SURPRISE */
}

/* border-box (intuitive) */
.box {
  box-sizing: border-box;
  width: 200px;
  padding: 20px;
  border: 2px solid;
  /* actual width = exactly 200px ← PREDICTABLE */
}
```

## Best Practice (always add this)
```css
*, *::before, *::after {
  box-sizing: border-box;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <p><strong>content-box (default):</strong></p>
  <div style="box-sizing: content-box; width: 200px; padding: 20px; border: 4px solid #e74c3c; background: #fde8e8; margin-bottom: 15px;">
    width: 200px but renders as 248px
  </div>
  <p><strong>border-box:</strong></p>
  <div style="box-sizing: border-box; width: 200px; padding: 20px; border: 4px solid #2ecc71; background: #e8fde8;">
    width: 200px and renders as exactly 200px
  </div>
</body>
</html>
```
