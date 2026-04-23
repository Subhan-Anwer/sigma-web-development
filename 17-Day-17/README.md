# Sigma Web Development Course

## Tutorial # 17 | Mastering CSS Selectors

[![Sigma Web Development Course - Tutorial # 17 ](https://img.youtube.com/vi/1cEG1T8beO4/maxresdefault.jpg "Mastering CSS Selectors")](https://www.youtube.com/watch?v=1cEG1T8beO4&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=17)

---

## Mastering CSS Selectors

There are multiple ways to select an element to apply styling for example select by id, class, element name etc.

---

## Select Element by Name

Selecting element by its name is most straight forward approach.

**Example:**

_HTML_

```html
<div>This is a div</div>
```

_CSS_

```css
div {
  /* Property: Value */
  background-color: red;
}
```

<br>

> This is about Element's Original Name not name attribute of an element eg name="custom-name"

The drawback of using this selection method is that you cant control which particular element to select or not. Example: if you select a div by its element name all of the div on the entire file gets selected and gets same styling whether you want it or not.
