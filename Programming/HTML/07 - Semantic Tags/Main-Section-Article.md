# `<main>`, `<section>`, `<article>`

## Tags

| Tag | Purpose |
|-----|---------|
| `<main>` | The primary content of the page (only one per page) |
| `<section>` | A thematic group of content |
| `<article>` | Self-contained, independently shareable content |

## Example
```html
<main>

  <section>
    <h2>Latest News</h2>

    <article>
      <h3>Article Title One</h3>
      <p>Published: 2024-01-01</p>
      <p>Summary of the first article...</p>
    </article>

    <article>
      <h3>Article Title Two</h3>
      <p>Published: 2024-01-02</p>
      <p>Summary of the second article...</p>
    </article>
  </section>

  <section>
    <h2>About Us</h2>
    <p>We are a team of developers...</p>
  </section>

</main>
```

## Notes
- Only **one `<main>`** per page
- `<article>` = could stand alone (blog post, news item, comment)
- `<section>` = related content grouped together (not standalone)
