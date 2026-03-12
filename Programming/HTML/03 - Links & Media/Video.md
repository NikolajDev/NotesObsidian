# `<video>` – Video

## Description
Embeds a video player directly in the page.

## Syntax
```html
<video src="video.mp4" controls></video>
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `src` | Video file path |
| `controls` | Show play/pause/volume controls |
| `autoplay` | Start automatically (use with `muted`) |
| `muted` | Mute by default |
| `loop` | Repeat video |
| `poster` | Image shown before video plays |
| `width` / `height` | Dimensions |

## Examples
```html
<!-- Basic video with controls -->
<video src="movie.mp4" controls width="640" height="360"></video>

<!-- Multiple formats for compatibility -->
<video controls width="640" poster="thumbnail.jpg">
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.webm" type="video/webm">
  Your browser does not support video.
</video>

<!-- Background video (autoplay, muted, loop) -->
<video autoplay muted loop>
  <source src="background.mp4" type="video/mp4">
</video>
```

## Notes
- `autoplay` requires `muted` to work in most browsers
- Always provide fallback text inside `<video>` tags
- Supported formats: MP4, WebM, OGG
