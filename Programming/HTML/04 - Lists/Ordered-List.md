# `<ol>` – Ordered List

## Description
A numbered list of items where order matters.

## Syntax
```html
<ol>
  <li>Item</li>
</ol>
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `type` | `1` (default), `A`, `a`, `I`, `i` |
| `start` | Start numbering from a specific number |
| `reversed` | Count down instead of up |

## Example
```html
<!-- Default numbered -->
<ol>
  <li>Boil water</li>
  <li>Add pasta</li>
  <li>Cook for 10 minutes</li>
</ol>

<!-- Uppercase letters -->
<ol type="A">
  <li>Option A</li>
  <li>Option B</li>
</ol>

<!-- Start from 5 -->
<ol start="5">
  <li>Fifth item</li>
  <li>Sixth item</li>
</ol>
```

## Notes
- Use for steps, rankings, instructions
- Use `<ul>` when order doesn't matter
