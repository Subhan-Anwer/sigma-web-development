# Sigma Web Development Course

## Tutorial # 23 | Display Property in CSS

[![Sigma Web Development Course - Tutorial # 23 ](https://img.youtube.com/vi/hRHV5cjEB1w/maxresdefault.jpg "Display Property in CSS")](https://www.youtube.com/watch?v=hRHV5cjEB1w&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=23)

---

## Display Property in CSS

The `display` property is important in CSS propert as it controls how the display of an elements is appeared in the layout of a webpage. The `display` property can take several values such as _`block`_, _`inline`_, _`inline-block`_, _`flex`_, _`grid`_, and more.

Every HTML element has a default display value and its generally **inline** or **block**.

<br>

## Common display Values

The CSS `display` property has many values. The following table lists the most commonly used:

| Value | Description |
|-------|-------------|
| `inline` | Displays the element as an inline element |
| `block` | Displays the element as a block element |
| `inline-block` | Displays the element as an inline-level element block container. The element itself is formatted as an inline element, but you can apply height, width, padding, and margin values unline _inline_ property |
| `flex` | Displays the element as a block-level flex container |
| `grid` | Displays the element as a block-level grid container |
| `none` | The element is completely hidden from the document flow (_does not take up any space_). |

---

## Visibility vs Hide

When you use `display: none;` the element is completely hidden from the page and does not take up any space. It acts like its not even there.

It is commonly used with JavaScript to hide or show elements without deleting and recreating them.

You can also use `visibility: hidden;` to hide an element.

However, with this property, the element will be hidden, but it will still take up the same space as if it was visible. Just like a ghost that is not visible but you can feel its presence in real life and here by seeing the blank space where the element would be.

### Quick Comparison

| Property | Description |
|----------|-------------|
| `display: none` | Completely hides the element and removes it from the document flow |
| `visibility: hidden` | Hides the element but keeps its space in the layout |

---

### Resource for More Information
-  [MDN Web Docs - display](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/display "MDN Docs Link")