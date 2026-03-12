# `<dl>` – Description List

## Description
A list of terms with their descriptions. Good for glossaries, FAQs, metadata.

## Tags

| Tag | Purpose |
|-----|---------|
| `<dl>` | Description list container |
| `<dt>` | Term (definition title) |
| `<dd>` | Description (definition detail) |

## Syntax
```html
<dl>
  <dt>Term</dt>
  <dd>Description of the term</dd>
</dl>
```

## Example
```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language — used to structure web content.</dd>

  <dt>CSS</dt>
  <dd>Cascading Style Sheets — used to style web pages.</dd>

  <dt>JavaScript</dt>
  <dd>A programming language for interactive web content.</dd>
</dl>
```

## Notes
- Less common than `<ul>` and `<ol>` but useful for key-value pairs
- One `<dt>` can have multiple `<dd>` elements
