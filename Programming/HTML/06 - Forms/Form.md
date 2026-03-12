# `<form>` – Form

## Description
Container for user input elements. Collects and submits data to a server.

## Syntax
```html
<form action="/submit" method="POST">
  <!-- inputs here -->
</form>
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `action` | URL where form data is sent |
| `method` | `GET` (visible in URL) or `POST` (hidden) |
| `enctype` | For file uploads: `multipart/form-data` |
| `novalidate` | Disable browser validation |

## Example
```html
<form action="/register" method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required>

  <button type="submit">Register</button>
</form>
```

## Notes
- Use `POST` for sensitive data (passwords, forms)
- Use `GET` for search forms (URL stays shareable)
- Always pair `<label>` with inputs using `for` + `id`
