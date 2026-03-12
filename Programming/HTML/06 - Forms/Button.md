# `<button>` – Button

## Description
A clickable button. More flexible than `<input type="submit">`.

## Syntax
```html
<button type="submit">Click me</button>
```

## Types

| Type | Behavior |
|------|----------|
| `submit` | Submits the form (default) |
| `reset` | Resets all form fields |
| `button` | No default action (use with JavaScript) |

## Examples
```html
<!-- Submit form -->
<button type="submit">Submit</button>

<!-- Reset form -->
<button type="reset">Clear</button>

<!-- JS button -->
<button type="button" onclick="alert('Hello!')">Click me</button>

<!-- Button with icon text -->
<button type="button">🔍 Search</button>

<!-- Disabled button -->
<button type="submit" disabled>Can't click</button>
```

## Notes
- Prefer `<button>` over `<input type="submit">` — can contain HTML inside
- Always specify `type` to avoid unexpected form submissions
