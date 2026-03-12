# `<a>` – Anchor (Link)

## Description
Creates a hyperlink to another page, file, or location.

## Syntax
```html
<a href="url">Link text</a>
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `href` | Destination URL |
| `target` | Where to open: `_blank` (new tab), `_self` (same tab) |
| `rel` | Relationship: `noopener noreferrer` for external links |
| `title` | Tooltip on hover |

## Examples
```html
<!-- External link -->
<a href="https://google.com" target="_blank" rel="noopener noreferrer">Google</a>

<!-- Internal link -->
<a href="/about.html">About Us</a>

<!-- Link to section on same page -->
<a href="#contact">Go to Contact</a>
<section id="contact">Contact info here</section>

<!-- Email link -->
<a href="mailto:hello@example.com">Send Email</a>

<!-- Phone link -->
<a href="tel:+421900000000">Call Us</a>
```

## Notes
- Always use `rel="noopener noreferrer"` with `target="_blank"` for security
- `href="#"` is a placeholder link (goes nowhere)
