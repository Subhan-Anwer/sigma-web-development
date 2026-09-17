# Sigma Web Development Course

## Tutorial # 35 | More on CSS Selectors

[![Sigma Web Development Course - Tutorial # 35 - More on CSS Selectors ](https://img.youtube.com/vi/L8NfSewTfxY/maxresdefault.jpg "More on CSS Selectors")](https://www.youtube.com/watch?v=L8NfSewTfxY&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=35)

---

## Select all childs of a parent

```css
div * {
    background-color: black;
    color: red;
}
```

---

## Attribute Selectors

```html
<p disabled=true>lorem ipsum dolor sit amet consectetur.</p>
```

```css

[disabled=true] {
    background-color: #f1f1f1;
    cursor: not-allowed;
    color: #a0a0a0;
}
```

---

## CSS before and after pseudo elements

```css
h1::before {
    content: "Hello! This is the content before heading";
}
```

```css
h1::after {
    content: "Hello! This is the content after heading";
}

```

---