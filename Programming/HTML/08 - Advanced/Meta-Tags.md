# `<meta>` – Meta Tags

## Description
Provide metadata about the HTML document. Placed inside `<head>`.
Not visible on the page but important for SEO, browsers, and social media.

## Common Meta Tags
```html
<head>
  <!-- Character encoding -->
  <meta charset="UTF-8">

  <!-- Responsive design -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Page description (shown in Google results) -->
  <meta name="description" content="Learn HTML basics step by step.">

  <!-- Keywords (less important now) -->
  <meta name="keywords" content="HTML, web development, tutorial">

  <!-- Author -->
  <meta name="author" content="John Doe">

  <!-- Refresh page every 30 seconds -->
  <meta http-equiv="refresh" content="30">

  <!-- Open Graph (social media previews) -->
  <meta property="og:title" content="My Page Title">
  <meta property="og:description" content="Page description for social media.">
  <meta property="og:image" content="https://example.com/image.jpg">
</head>
```

## Notes
- `charset="UTF-8"` — always include, supports all characters
- `viewport` — required for mobile responsive design
- `og:` tags control how your page looks when shared on Facebook, Slack etc.
