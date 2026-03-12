# Table – `colspan` & `rowspan`

## Description
Merge multiple cells together horizontally or vertically.

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `colspan` | Merge cells horizontally (across columns) |
| `rowspan` | Merge cells vertically (across rows) |

## colspan Example
```html
<table border="1">
  <tr>
    <td colspan="3">Merged across 3 columns</td>
  </tr>
  <tr>
    <td>Col 1</td>
    <td>Col 2</td>
    <td>Col 3</td>
  </tr>
</table>
```

## rowspan Example
```html
<table border="1">
  <tr>
    <td rowspan="2">Merged 2 rows</td>
    <td>Row 1, Col 2</td>
  </tr>
  <tr>
    <td>Row 2, Col 2</td>
  </tr>
</table>
```

## Combined Example
```html
<table border="1">
  <tr>
    <th colspan="2">Name</th>
    <th>Score</th>
  </tr>
  <tr>
    <td>First</td>
    <td>Last</td>
    <td rowspan="2">Same score</td>
  </tr>
  <tr>
    <td>John</td>
    <td>Doe</td>
  </tr>
</table>
```
