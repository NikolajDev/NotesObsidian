# `<header>`, `<nav>`, `<footer>`

## Description
Semantic HTML5 elements that describe the role of content clearly.

## Tags

| Tag | Purpose |
|-----|---------|
| `<header>` | Introductory content, logo, heading |
| `<nav>` | Navigation links |
| `<footer>` | Footer info, copyright, links |

## Example
```html
<!DOCTYPE html>
<html lang="en">
<body>

  <header>
    <h1>My Website</h1>
    <p>Welcome to my page</p>
  </header>

  <nav>
    <a href="/">Home</a>
    <a href="/about">About</a>
    <a href="/contact">Contact</a>
  </nav>

  <main>
    <p>Main content goes here.</p>
  </main>

  <footer>
    <p>&copy; 2024 My Website. All rights reserved.</p>
  </footer>

</body>
</html>
```

## Notes
- These are **semantic** — they describe meaning, not just structure
- A page can have multiple `<header>` and `<footer>` (e.g. inside `<article>`)
- `<nav>` should only be used for major navigation blocks
