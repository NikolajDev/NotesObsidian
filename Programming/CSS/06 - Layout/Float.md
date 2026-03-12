# Float

## Description
Removes element from normal flow and pushes it left or right.
Mostly replaced by Flexbox and Grid, but still used for text wrapping around images.

## Example
```css
/* Float image left, text wraps around */
img {
  float: left;
  margin: 0 20px 10px 0;
}

/* Clear float — stop wrapping */
.clearfix::after {
  content: "";
  display: block;
  clear: both;
}

/* Float elements side by side (old technique) */
.column {
  float: left;
  width: 33.33%;
  padding: 10px;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    .clearfix::after { content: ""; display: block; clear: both; }
  </style>
</head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <div class="clearfix" style="border: 1px solid #ddd; padding: 15px; border-radius: 4px;">
    <div style="float: left; width: 80px; height: 80px; background: #3498db; border-radius: 4px; margin: 0 15px 5px 0;"></div>
    <p>This text wraps around the floated blue box on the left. Float was the classic way to create layouts before Flexbox and Grid existed. It is still useful for wrapping text around images like in a magazine layout.</p>
  </div>
</body>
</html>
```

## Notes
- Always clear floats to prevent layout collapse
- Prefer **Flexbox or Grid** for layouts
- Float is still valid for text wrapping around images
