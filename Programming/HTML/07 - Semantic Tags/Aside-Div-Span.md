# `<aside>`, `<div>`, `<span>`

## Tags

| Tag | Type | Purpose |
|-----|------|---------|
| `<aside>` | Block | Secondary content (sidebar, tips) |
| `<div>` | Block | Generic container, no semantic meaning |
| `<span>` | Inline | Generic inline container |

## `<aside>` Example
```html
<main>
  <article>
    <h2>Main Article</h2>
    <p>Main content here...</p>
  </article>

  <aside>
    <h3>Related Links</h3>
    <ul>
      <li><a href="#">Link 1</a></li>
      <li><a href="#">Link 2</a></li>
    </ul>
  </aside>
</main>
```

## `<div>` Example
```html
<!-- Layout wrapper -->
<div class="container">
  <div class="card">
    <h2>Card Title</h2>
    <p>Card content.</p>
  </div>
</div>
```

## `<span>` Example
```html
<p>The price is <span style="color: green; font-weight: bold;">$9.99</span> today.</p>
<p>Status: <span class="badge">Active</span></p>
```

## Notes
- Use semantic tags (`<aside>`, `<section>`) when possible
- Use `<div>` only when no semantic tag fits
- `<span>` is the inline version of `<div>`
