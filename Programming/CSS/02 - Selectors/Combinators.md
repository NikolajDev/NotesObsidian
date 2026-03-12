# Combinators

## Description
Combine selectors to target elements based on their relationship in the HTML tree.

## Types

| Combinator | Syntax | Targets |
|------------|--------|---------|
| Descendant | `A B` | B inside A (any depth) |
| Child | `A > B` | B that is direct child of A |
| Adjacent sibling | `A + B` | B immediately after A |
| General sibling | `A ~ B` | All B after A |

## Example
```css
/* Descendant: all <a> inside .nav */
.nav a {
  color: white;
  text-decoration: none;
}

/* Child: only direct <li> children of <ul> */
ul > li {
  list-style: square;
}

/* Adjacent sibling: <p> right after <h2> */
h2 + p {
  font-size: 1.1em;
  color: #555;
}

/* General sibling: all <p> after .intro */
.intro ~ p {
  border-left: 3px solid #ccc;
  padding-left: 10px;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    .nav a { color: white; text-decoration: none; }
    .nav { background: #333; padding: 10px; }
    h2 + p { font-size: 1.1em; color: #555; font-style: italic; }
    .intro ~ p { border-left: 3px solid #ccc; padding-left: 10px; }
  </style>
</head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <nav class="nav">
    <a href="#">Home</a> |
    <a href="#">About</a> |
    <a href="#">Contact</a>
  </nav>
  <br>
  <h2>Heading</h2>
  <p>This paragraph is right after h2 — styled with adjacent sibling.</p>
  <p class="intro">Intro paragraph</p>
  <p>This follows .intro — general sibling selector applies.</p>
  <p>This also follows .intro.</p>
</body>
</html>
```
