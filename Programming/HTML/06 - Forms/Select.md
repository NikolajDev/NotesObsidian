# `<select>` – Dropdown

## Description
A dropdown menu for selecting one or multiple options.

## Syntax
```html
<select name="choice">
  <option value="1">Option 1</option>
  <option value="2">Option 2</option>
</select>
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `name` | Form field name |
| `multiple` | Allow multiple selections |
| `size` | Number of visible options |
| `required` | Field is required |

## Examples
```html
<!-- Basic dropdown -->
<select name="country">
  <option value="">-- Select country --</option>
  <option value="sk">Slovakia</option>
  <option value="cz">Czech Republic</option>
  <option value="us">United States</option>
</select>

<!-- Grouped options -->
<select name="car">
  <optgroup label="European">
    <option value="skoda">Skoda</option>
    <option value="vw">Volkswagen</option>
  </optgroup>
  <optgroup label="American">
    <option value="ford">Ford</option>
  </optgroup>
</select>

<!-- Multi-select -->
<select name="skills" multiple size="4">
  <option value="html">HTML</option>
  <option value="css">CSS</option>
  <option value="js">JavaScript</option>
  <option value="py">Python</option>
</select>
```
