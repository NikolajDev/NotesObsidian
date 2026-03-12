# `<textarea>` – Multi-line Text Input

## Description
A resizable multi-line text input for longer content like messages or comments.

## Syntax
```html
<textarea name="message" rows="4" cols="50"></textarea>
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `name` | Form field name |
| `rows` | Visible number of lines |
| `cols` | Visible width in characters |
| `placeholder` | Hint text |
| `maxlength` | Max characters allowed |
| `readonly` | Read-only field |
| `disabled` | Disabled field |
| `resize` | Controlled via CSS |

## Example
```html
<label for="message">Your message:</label>
<textarea
  id="message"
  name="message"
  rows="6"
  cols="50"
  placeholder="Write your message here..."
  maxlength="500"
  required
></textarea>

<!-- Disable resizing with CSS -->
<textarea style="resize: none;" rows="4" name="bio"></textarea>
```

## Notes
- Unlike `<input>`, `<textarea>` has a closing tag
- Default value goes between the tags (not in `value` attribute)
- Use CSS `resize: none` to prevent user resizing
