# How to Add CSS

## 3 Ways to Add CSS

### 1. Inline CSS
Directly on the element using the `style` attribute.
```html
<p style="color: red; font-size: 18px;">Red paragraph</p>
```

### 2. Internal CSS
Inside a `<style>` tag in the `<head>`.
```html
<head>
  <style>
    p {
      color: red;
      font-size: 18px;
    }
  </style>
</head>
```

### 3. External CSS (recommended)
A separate `.css` file linked in `<head>`.
```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```
```css
/* styles.css */
p {
  color: red;
  font-size: 18px;
}
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    .internal { color: green; font-weight: bold; }
  </style>
</head>
<body>
  <p style="color: red; font-size: 18px;">1. Inline CSS – red text</p>
  <p class="internal">2. Internal CSS – green bold text</p>
  <p style="color: blue;">3. Would be External CSS – shown here as inline</p>
</body>
</html>
```

## Priority (highest to lowest)
1. Inline styles
2. Internal `<style>` tag
3. External stylesheet
4. Browser defaults

## Notes
- Always prefer **external CSS** for real projects
- Inline CSS is useful for quick tests or dynamic styles via JavaScript
