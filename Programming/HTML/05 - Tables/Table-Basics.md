# `<table>` – Table Basics

## Description
Used to display data in rows and columns.

## Core Tags

| Tag | Purpose |
|-----|---------|
| `<table>` | Table container |
| `<tr>` | Table row |
| `<td>` | Table data cell |
| `<th>` | Table header cell (bold + centered) |

## Syntax
```html
<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
</table>
```

## Example
```html
<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>City</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>25</td>
    <td>New York</td>
  </tr>
  <tr>
    <td>Bob</td>
    <td>30</td>
    <td>London</td>
  </tr>
</table>
```

## Notes
- Use CSS for styling, not the `border` attribute (deprecated)
- Tables are for **data**, not page layout
