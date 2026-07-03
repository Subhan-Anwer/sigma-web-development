# Sigma Web Development Course

## Tutorial # 26 | CSS Overflow Property

[![Sigma Web Development Course - Tutorial # 26 ](https://img.youtube.com/vi/ntlawluDB-c/maxresdefault.jpg "CSS Overflow Property")](https://www.youtube.com/watch?v=ntlawluDB-c&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=24)

---

## CSS Overflow Property

### Overview

The **`overflow`** property controls how content that exceeds an element’s box is handled. It determines whether the excess is visible, clipped, or scrollable, affecting both layout and user experience.

### Values

- `visible` – The default. Content overflows the box and remains visible.
- `hidden` – Clips the overflowing content; no scrollbars are provided.
- `scroll` – Always shows scrollbars, allowing the user to scroll to see hidden content.
- `auto` – Scrollbars appear only when necessary (i.e., when content actually overflows).

### Axis‑Specific Properties
- `overflow-x` – Controls horizontal overflow.
- `overflow-y` – Controls vertical overflow.

### Example
```html
<div class="box">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec a diam lectus.</p>
</div>
```
```css
.box {
  width: 300px;
  height: 150px;
  padding: 1rem;
  border: 2px solid #4a90e2;
  overflow: auto; /* Show scrollbars only when needed */
}
```
The container above will display scrollbars if the paragraph exceeds the set dimensions.

### Tips
- Use `overflow: hidden` to create CSS‑only image cropping or mask effects.
- When using `overflow: scroll`, note that scrollbars are always visible, which can affect layout aesthetics.
- Combining `overflow-x` and `overflow-y` with different values enables fine‑grained control (e.g., `overflow-x: hidden; overflow-y: auto;`).

---
