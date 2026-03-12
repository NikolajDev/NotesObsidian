# `<ul>` – Unordered List

## Description
A list of items with bullet points (no specific order).

## Syntax
```html
<ul>
  <li>Item</li>
</ul>
```

## Example
```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>

<!-- Nested list -->
<ul>
  <li>Frontend
    <ul>
      <li>HTML</li>
      <li>CSS</li>
    </ul>
  </li>
  <li>Backend</li>
</ul>
```

## Notes
- `<ul>` = unordered list (bullet points)
- `<li>` = list item
- Can be nested inside other `<li>` elements
- Default bullet style can be changed with CSS: `list-style-type: square;`
