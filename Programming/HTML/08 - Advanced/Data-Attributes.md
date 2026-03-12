# Data Attributes – `data-*`

## Description
Custom attributes to store extra data on HTML elements.
Used heavily with JavaScript.

## Syntax
```html
<element data-yourname="value"></element>
```

## Example
```html
<!-- Store extra info on elements -->
<button data-user-id="42" data-action="delete">Delete User</button>

<div data-category="electronics" data-price="299">
  Laptop Pro
</div>

<!-- List with data attributes -->
<ul>
  <li data-id="1" data-status="active">Alice</li>
  <li data-id="2" data-status="inactive">Bob</li>
  <li data-id="3" data-status="active">Carol</li>
</ul>
```

## Accessing with JavaScript
```javascript
const btn = document.querySelector('button');

// Get value
console.log(btn.dataset.userId);   // "42"
console.log(btn.dataset.action);   // "delete"

// Set value
btn.dataset.action = "edit";

// CSS can also use data attributes
// button[data-action="delete"] { background: red; }
```

## Notes
- Name must start with `data-` followed by at least one character
- Use lowercase and hyphens: `data-user-id` not `data-userId`
- Accessed in JS via `element.dataset.userId` (camelCase conversion)
- Great for passing data to JavaScript without hidden inputs
