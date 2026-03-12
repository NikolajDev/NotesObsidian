# Class & ID Selectors

## Description

| Selector | Syntax | Use |
|----------|--------|-----|
| Class | `.classname` | Reusable, multiple elements |
| ID | `#idname` | Unique, one element per page |

## Syntax
```css
/* Class selector */
.highlight {
  background-color: yellow;
  font-weight: bold;
}

/* ID selector */
#main-title {
  font-size: 3rem;
  color: navy;
  text-align: center;
}

/* Combining: element + class */
p.note {
  border-left: 4px solid orange;
  padding-left: 10px;
}
```

## HTML Usage
```html
<h1 id="main-title">Page Title</h1>
<p class="highlight">This is highlighted.</p>
<p class="highlight note">This has two classes.</p>
<p>Normal paragraph.</p>
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"></head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <h1 style="font-size: 3rem; color: navy; text-align: center;">ID Selector – Main Title</h1>
  <p style="background-color: yellow; font-weight: bold;">Class selector – highlighted text</p>
  <p style="background-color: yellow; font-weight: bold; border-left: 4px solid orange; padding-left: 10px;">Two classes: highlight + note</p>
  <p>Normal paragraph – no class applied.</p>
</body>
</html>
```

## Notes
- Use `class` for styles you reuse, `id` for unique elements
- An element can have **multiple classes**: `class="btn btn-primary"`
- ID has higher specificity than class
