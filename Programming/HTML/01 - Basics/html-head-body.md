# `<html>`, `<head>`, `<body>`

## Description
The three root elements of every HTML page.

## Syntax
```html
<html lang="en">
  <head>
    <!-- metadata, title, links to CSS -->
  </head>
  <body>
    <!-- visible content -->
  </body>
</html>
```

## Elements

| Tag | Purpose |
|-----|---------|
| `<html>` | Root element, wraps everything |
| `<head>` | Metadata – not visible on page |
| `<body>` | All visible content goes here |

## Example
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Title</title>
  </head>
  <body>
    <h1>Visible Heading</h1>
    <p>Visible paragraph.</p>
  </body>
</html>
```

## Notes
- `lang="en"` helps screen readers and SEO
- Everything in `<head>` is invisible to the user
