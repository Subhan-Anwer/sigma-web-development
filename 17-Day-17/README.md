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

---

## Select Element by Class

Selecting element by given **`class`** is the recommended method of selecting and giving styling to a single or group of elements falls under the same class. Heres how to do it.

```html
<div class="red">This is a div with "red" class</div>
```

```css
.red {
  background-color: red;
}
```

---

## Select Element by ID

We can also select elements by their **`ID`** attribute. however id is mostly used for javascript logic not for selecting for styling through css.

**Example:**

```html
<p id="blue-para">Lorem ipsum</p>
```

```css
#blue-para {
  background-color: lightblue;
  color: darkblue;
}
```

---

## Select a Child Element of a Parent

If we want to make a condition to select the child of a parent or we want to select an element without class or id we can wrap it in a parent tag and select it to give styling specifically to only that child element of specified parent element.

Heres how to do it.

```html
<div>
  This is Parent Div of Paragraph

  <p>This is a Child of Parent Div</p>
</div>
```

```css
div > p {
  text-decoration: underline;
  background-color: aqua;
}
```

Here **`<div>`** is a parent element and **`<p>`** is the child element of **`<div>`**.

---

## Select Descendant Element

In child selector the **`>`** symbol stricts to only the direct child of the parent element, but if we want it to be flexible and select the descendant of the parent whether its wrapped inside another element, we can use _descendant selector_.

its simple just remove the **`>`**, Heres how to do it.

```html
<div>
  This is Parent Div of Paragraph. Childs are: article and paragraph.

  <article>
    <p>This is a Child of Parent Div</p>
  </article>
</div>
```

```css
div p {
  text-decoration: underline;
  background-color: aqua;
}
```