# Grid Template Areas

## Description
Name areas of the grid for a visual, readable layout.

## Syntax
```css
.container {
  display: grid;
  grid-template-columns: 200px 1fr;
  grid-template-rows: auto 1fr auto;
  grid-template-areas:
    "header  header"
    "sidebar main"
    "footer  footer";
  gap: 12px;
  min-height: 100vh;
}

.header  { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main    { grid-area: main; }
.footer  { grid-area: footer; }
```

## Empty Cells
Use `.` for an empty cell:
```css
grid-template-areas:
  "header header"
  ".      main  "
  "footer footer";
```

## Preview
```html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8">
  <style>
    .layout {
      display: grid;
      grid-template-columns: 150px 1fr;
      grid-template-areas:
        "header  header"
        "sidebar main"
        "footer  footer";
      gap: 10px;
    }
    .g-header  { grid-area: header; }
    .g-sidebar { grid-area: sidebar; }
    .g-main    { grid-area: main; }
    .g-footer  { grid-area: footer; }
  </style>
</head>
<body style="font-family: Arial, sans-serif; padding: 20px;">
  <div class="layout">
    <div class="g-header" style="background: #2c3e50; color: white; padding: 15px; border-radius: 4px; text-align: center;">Header</div>
    <div class="g-sidebar" style="background: #8e44ad; color: white; padding: 15px; border-radius: 4px; text-align: center;">Sidebar</div>
    <div class="g-main" style="background: #3498db; color: white; padding: 30px; border-radius: 4px; text-align: center;">Main Content</div>
    <div class="g-footer" style="background: #7f8c8d; color: white; padding: 15px; border-radius: 4px; text-align: center;">Footer</div>
  </div>
</body>
</html>
```
