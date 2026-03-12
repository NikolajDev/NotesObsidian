# Element Selector

## Description
Targets all HTML elements of a specific type.

## Syntax
```css
element {
  property: value;
}
```

## Example
```css
h1 {
  color: darkblue;
  font-size: 2rem;
}

p {
  color: #444;
  line-height: 1.7;
}

a {
  color: coral;
  text-decoration: none;
}

/* Universal selector — targets everything */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <h1 style="color: darkblue; font-size: 2rem;">Element Selector on h1</h1>
  <p style="color: #444; line-height: 1.7;">This paragraph is styled using the <code>p</code> element selector.</p>
  <p style="color: #444; line-height: 1.7;">All paragraphs get the same style automatically.</p>
  <a href="#" style="color: coral; text-decoration: none;">This link is styled with the a selector</a>
</body>
</html>
```

## Notes
- Affects **all** matching elements on the page
- `*` (universal selector) targets every element — use carefully
