# Sigma Web Development Course

## Tutorial # 34 | CSS Float & Clear

[![Sigma Web Development Course - Tutorial # 34 - CSS Float & Clear ](https://img.youtube.com/vi/6_UoTF7njLM/maxresdefault.jpg "CSS Float & Clear")](https://www.youtube.com/watch?v=6_UoTF7njLM&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=34)

---

## What is Float & Why to use it?

After the flexbox has came, the use of `Float` and `Clear` has significantly dropped. But if a clients come to you with its old website which has `Float` & `Clear` so you need to have the understanding of its concept.

## CSS Float Property

The `float` property specifies how an element should `float` within its container.

It places an element on the left or right side of its container, allowing text and inline elements to wrap around it.

### Float Property Values

The `float` property can have one of the following values:

- `left` - The element floats to the left of its container
- `right` - The element floats to the right of its container
- `none` - Default. The element does not float and is displayed just where it occurs in the text
inherit - The element inherits the float value of its parent

> **Tip:** The float property is often used to wrap text around images!

### CSS Float Examples:

For CSS float examples, see [index.html](./index.html)

---

## CSS Clear Property

The `clear` property is used to clear the float property and specifies which sides the element should not float next to.

For example if we use `clear: right;`, on an inline element then no other element which has `float: right` can float to this element's right side.

In simple words, when one element of a container has `clear` property, it is saying to all elements of the container to strictly not to flow on the specified side of it.

### Clear Property Values

The `clear` propert can have one of the following values:

- `left` - An element with `float: left` will not float to this element's left side.
- `right` - An element with `float: right` will not float to this element's right side.
- `none` - Default. An element with float property can float to the left or right side of this element.
- `both` - An element with float property will not float to the left or right side of this element.

### CSS Clear Examples:

For CSS clear examples, see [index.html](./index.html)