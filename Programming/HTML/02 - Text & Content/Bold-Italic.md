# Bold & Italic

## Tags

| Tag | Meaning | Result |
|-----|---------|--------|
| `<strong>` | Important text (semantic) | **bold** |
| `<b>` | Bold (visual only) | **bold** |
| `<em>` | Emphasized text (semantic) | *italic* |
| `<i>` | Italic (visual only) | *italic* |

## Syntax
```html
<strong>Important text</strong>
<b>Bold text</b>
<em>Emphasized text</em>
<i>Italic text</i>
```

## Example
```html
<p>This is <strong>very important</strong> information.</p>
<p>The term <em>HTML</em> stands for HyperText Markup Language.</p>
<p>Use <b>bold</b> for styling, <strong>strong</strong> for importance.</p>
<p>Book titles like <i>The Great Gatsby</i> use italic.</p>
```

## Notes
- Prefer `<strong>` over `<b>` and `<em>` over `<i>` for semantic meaning
- Screen readers treat `<strong>` and `<em>` with emphasis
