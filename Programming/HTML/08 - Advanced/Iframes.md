# `<iframe>` – Inline Frame

## Description
Embeds another HTML page or external content (maps, videos) inside your page.

## Syntax
```html
<iframe src="url" width="600" height="400"></iframe>
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `src` | URL to embed |
| `width` / `height` | Dimensions |
| `title` | Accessibility description |
| `allowfullscreen` | Allow fullscreen (for videos) |
| `loading` | `lazy` for performance |
| `sandbox` | Restrict permissions |

## Examples
```html
<!-- Embed a webpage -->
<iframe
  src="https://example.com"
  width="800"
  height="500"
  title="Example website"
></iframe>

<!-- YouTube video -->
<iframe
  width="560"
  height="315"
  src="https://www.youtube.com/embed/dQw4w9WgXcQ"
  title="YouTube video"
  allowfullscreen
></iframe>

<!-- Google Maps -->
<iframe
  src="https://maps.google.com/maps?q=Bratislava&output=embed"
  width="600"
  height="450"
  loading="lazy"
  title="Map of Bratislava"
></iframe>
```

## Notes
- Always add `title` attribute for accessibility
- `sandbox` attribute increases security for untrusted content
- Some websites block being embedded with `X-Frame-Options`
