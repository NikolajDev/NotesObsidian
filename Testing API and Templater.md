# HTML – Basics

## What is HTML?
HTML (HyperText Markup Language) is a markup language for creating web pages. The browser reads HTML and displays the content.

---

## Basic Structure
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Page Title</title>
  </head>
  <body>
    <h1>Hello World!</h1>
  </body>
</html>
```
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Page Title</title>
  </head>
  <body>
    <h1>Hello World!</h1>
  </body>
</html>

---

## Headings
```html
<h1>Largest heading</h1>
<h2>Second level</h2>
<h3>Third level</h3>
<!-- up to h6 -->
```

<h1>Largest heading</h1>
<h2>Second level</h2>
<h3>Third level</h3>
---

## Text
```html
<p>Paragraph of text</p>
<strong>Bold text</strong>
<em>Italic text</em>
<br>         <!-- line break -->
<hr>         <!-- horizontal line -->
```
<p>Paragraph of text</p>
<strong>Bold text</strong>
<em>Italic text</em>
<br> 
<hr>

## Links and Images
```html
<!-- Link -->
<a href="https://example.com" target="_blank">Click here</a>

<!-- Image -->
<img src="image.jpg" alt="Image description" width="300">
```
<a href="https://example.com" target="_blank">Click here</a>
<img src="image.jpg" alt="Image description" width="300">
---

## Lists
```html
<!-- Unordered -->
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

<!-- Ordered -->
<ol>
  <li>First</li>
  <li>Second</li>
</ol>
```
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>
<ol>
  <li>First</li>
  <li>Second</li>
</ol>
---

## Tables
```html
<table>
  <thead>
    <tr>
      <th>Column 1</th>
      <th>Column 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Value 1</td>
      <td>Value 2</td>
    </tr>
  </tbody>
</table>
```
<table>
  <thead>
    <tr>
      <th>Column 1</th>
      <th>Column 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Value 1</td>
      <td>Value 2</td>
    </tr>
  </tbody>
</table>
---

## Div and Span
```html
<!-- Block container -->
<div class="box">
  <p>Content</p>
</div>

<!-- Inline container -->
<p>This is <span style="color: red;">red</span> text.</p>
```
<div class="box">
  <p>Content</p>
</div>
<p>This is <span style="color: red;">red</span> text.</p>

---

## Forms
```html
<form action="/submit" method="POST">
  <input type="text" placeholder="Name" name="name">
  <input type="email" placeholder="Email" name="email">
  <button type="submit">Submit</button>
</form>
```
<form action="/submit" method="POST">
  <input type="text" placeholder="Name" name="name">
  <input type="email" placeholder="Email" name="email">
  <button type="submit">Submit</button>
</form>
---

## Semantic Tags (HTML5)

| Tag         | Meaning      |
| ----------- | ------------ |
| `<header>`  | Page header  |
| `<nav>`     | Navigation   |
| `<main>`    | Main content |
| `<section>` | Section      |
| `<article>` | Article      |
| `<aside>`   | Sidebar      |
| `<footer>`  | Page footer  |

---

## Attributes
```html
<!-- Attributes give tags additional information -->
<a href="url" target="_blank" rel="noopener">Link</a>
<img src="img.jpg" alt="description" width="200" height="100">
<div id="unique" class="reusable"></div>
```
<a href="url" target="_blank" rel="noopener">Link</a>
<img src="img.jpg" alt="description" width="200" height="100">
<div id="unique" class="reusable" style="width:100px; height:100px; border: solid 2px red"></div>
---

## Comments
```html
<!-- This is a comment, the browser won't display it -->
```