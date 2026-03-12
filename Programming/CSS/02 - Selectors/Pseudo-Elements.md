# Pseudo-Elements

## Description
Target and style a **specific part** of an element.
Written with double colon `::`.

## Common Pseudo-Elements

| Pseudo-element | Targets |
|----------------|---------|
| `::before` | Insert content before element |
| `::after` | Insert content after element |
| `::first-line` | First line of text |
| `::first-letter` | First letter of text |
| `::placeholder` | Input placeholder text |
| `::selection` | Highlighted/selected text |

## Example
```css
/* Add content before/after */
.note::before {
  content: "📌 ";
}

.price::after {
  content: " USD";
  color: gray;
  font-size: 0.8em;
}

/* Style first letter (drop cap) */
p::first-letter {
  font-size: 3em;
  font-weight: bold;
  float: left;
  line-height: 1;
  margin-right: 5px;
}

/* Placeholder color */
input::placeholder {
  color: lightgray;
  font-style: italic;
}

/* Selection highlight color */
::selection {
  background-color: yellow;
  color: black;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    .note::before { content: "📌 "; }
    .price::after { content: " USD"; color: gray; font-size: 0.8em; }
    .dropcap::first-letter { font-size: 3em; font-weight: bold; float: left; line-height: 1; margin-right: 4px; }
    input::placeholder { color: lightgray; font-style: italic; }
  </style>
</head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <p class="note">This note has a pin icon added via ::before</p>
  <p>Price: <span class="price">9.99</span></p>
  <p class="dropcap">Drop cap example — the first letter of this paragraph is enlarged using ::first-letter pseudo-element.</p>
  <input type="text" placeholder="Italic placeholder text" style="padding: 6px; border: 1px solid #ccc;">
</body>
</html>
```
