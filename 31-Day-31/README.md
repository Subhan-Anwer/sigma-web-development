# Sigma Web Development Course

## Tutorial # 31 | CSS Media Queries

[![Sigma Web Development Course - Tutorial # 31 - CSS Media Queries ](https://img.youtube.com/vi/eHye3PxH4jU/maxresdefault.jpg "CSS Media Queries")](https://www.youtube.com/watch?v=eHye3PxH4jU&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=31)

---

## CSS Media Queries

In CSS media queries are used to apply different styles for different devices or screen sizes. They allow you to create responsive designs that adapt to various screen widths, orientations, and resolutions.

### Syntax
```css
@media not | only mediatype and (expressions) {
  CSS-Code;
}
```

> **Note:** The `not` keyword negates the media query, while the `only` keyword is used to apply styles only if the media type matches however its optional and generally we will not use it. The `mediatype` can be `all`, `print`, or `screen`. The `expressions` are conditions that define when the styles should be applied, we generally use the `screen` media type.

### Example
```css
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

If the screen width is maximum 600 pixels or less than 600 pixels, the background color of the body will change to light blue.