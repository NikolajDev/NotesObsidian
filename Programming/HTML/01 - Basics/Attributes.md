# HTML Attributes

## Description
Attributes provide additional information about HTML elements.
They are always placed inside the opening tag.

## Syntax
```html
<tag attribute="value">Content</tag>
```

## Common Attributes

| Attribute | Used on | Purpose |
|-----------|---------|---------|
| `id` | any | Unique identifier |
| `class` | any | CSS class name |
| `style` | any | Inline CSS styles |
| `href` | `<a>` | Link destination |
| `src` | `<img>`, `<script>` | File source |
| `alt` | `<img>` | Alternative text |
| `type` | `<input>`, `<button>` | Element type |
| `placeholder` | `<input>` | Hint text |
| `disabled` | form elements | Disables element |

## Example
```html
<!-- id and class -->
<div id="main-content" class="container highlight">
  Hello
</div>

<!-- href and target -->
<a href="https://example.com" target="_blank" rel="noopener">Visit</a>

<!-- src and alt -->
<img src="photo.jpg" alt="A photo of a cat" width="300">

<!-- style inline -->
<p style="color: red; font-size: 18px;">Red text</p>
```

## Notes
- `id` must be **unique** per page
- `class` can be reused on multiple elements
- Boolean attributes don't need a value: `<input disabled>`
