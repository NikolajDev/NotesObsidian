# `<audio>` – Audio

## Description
Embeds an audio player in the page.

## Syntax
```html
<audio src="audio.mp3" controls></audio>
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `src` | Audio file path |
| `controls` | Show player controls |
| `autoplay` | Play automatically |
| `muted` | Mute by default |
| `loop` | Repeat audio |

## Examples
```html
<!-- Basic audio -->
<audio src="music.mp3" controls></audio>

<!-- Multiple formats -->
<audio controls>
  <source src="music.mp3" type="audio/mpeg">
  <source src="music.ogg" type="audio/ogg">
  Your browser does not support audio.
</audio>

<!-- Autoplay loop (e.g. background music) -->
<audio src="ambient.mp3" autoplay loop muted></audio>
```

## Notes
- Supported formats: MP3, OGG, WAV
- Always provide fallback text
- Autoplay is blocked by most browsers unless muted
