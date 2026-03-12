# `<img>` – Image

## Description
Embeds an image into the page. Self-closing tag.

## Syntax
```html
<img src="path/to/image.jpg" alt="Description">
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `src` | Path or URL to the image |
| `alt` | Alternative text (accessibility + SEO) |
| `width` | Width in pixels or % |
| `height` | Height in pixels or % |
| `loading` | `lazy` = load only when visible |

## Examples
```html
<!-- Local image -->
<img src="images/photo.jpg" alt="A mountain landscape" width="600">

<!-- External image -->
<img src="https://picsum.photos/400/300" alt="Random photo">

<!-- Lazy loading -->
<img src="large-photo.jpg" alt="Large photo" loading="lazy">

<!-- Responsive image -->
<img src="photo.jpg" alt="Photo" style="max-width: 100%; height: auto;">
```

## Notes
- Always include `alt` — required for accessibility
- Empty `alt=""` for decorative images
- Prefer `max-width: 100%` over fixed width for responsive design
