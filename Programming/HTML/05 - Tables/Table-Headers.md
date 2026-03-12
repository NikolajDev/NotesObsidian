# Table Structure – `<thead>`, `<tbody>`, `<tfoot>`

## Description
Semantic grouping of table sections for better structure and accessibility.

## Tags

| Tag | Purpose |
|-----|---------|
| `<thead>` | Header rows |
| `<tbody>` | Main data rows |
| `<tfoot>` | Footer rows (totals, summaries) |

## Example
```html
<table>
  <thead>
    <tr>
      <th>Product</th>
      <th>Price</th>
      <th>Quantity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Apple</td>
      <td>$1.00</td>
      <td>5</td>
    </tr>
    <tr>
      <td>Banana</td>
      <td>$0.50</td>
      <td>10</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Total</td>
      <td>$10.00</td>
      <td>15</td>
    </tr>
  </tfoot>
</table>
```

## Notes
- `<thead>` and `<tfoot>` are optional but recommended
- Improves accessibility for screen readers
