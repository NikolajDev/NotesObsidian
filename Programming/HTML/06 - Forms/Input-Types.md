# `<input>` – Input Types

## Description
The most versatile form element. The `type` attribute controls its behavior.

## Common Types

| Type | Description |
|------|-------------|
| `text` | Single line text |
| `email` | Email address (validated) |
| `password` | Hidden text input |
| `number` | Numeric input |
| `checkbox` | Tick box |
| `radio` | Select one from group |
| `file` | File upload |
| `date` | Date picker |
| `range` | Slider |
| `hidden` | Hidden value |
| `submit` | Submit button |
| `reset` | Reset form |

## Examples
```html
<input type="text" placeholder="Your name" name="name">
<input type="email" placeholder="your@email.com" name="email">
<input type="password" placeholder="Password" name="pass">
<input type="number" min="0" max="100" name="age">
<input type="date" name="birthday">

<!-- Checkbox -->
<input type="checkbox" id="agree" name="agree">
<label for="agree">I agree to terms</label>

<!-- Radio buttons -->
<input type="radio" id="male" name="gender" value="male">
<label for="male">Male</label>
<input type="radio" id="female" name="gender" value="female">
<label for="female">Female</label>

<!-- File upload -->
<input type="file" name="avatar" accept="image/*">

<!-- Range slider -->
<input type="range" min="0" max="100" value="50" name="volume">
```
