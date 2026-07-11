# Sigma Web Development Course

## Tutorial # 28 | CSS Position Property

[![Sigma Web Development Course - Tutorial # 28 ](https://img.youtube.com/vi/cOw6tgH6P20/maxresdefault.jpg "CSS Overflow Property")](https://www.youtube.com/watch?v=cOw6tgH6P20&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=28)

---

## CSS Positioning
CSS positioning is about controlling the placement of elements within a web page.

With CSS positioning, you can override the normal document flow.

## Position Property in CSS

Position property is used to set the position of an element. It lets you set other properties as well which helps you to position an element accordingly. Without setting postion property you cant apply other properties to adjust a position of an element. By default, the position of an element is static and it prevents any top, bottom, left and right property. 

This property can have one of the following values:

| Position Value | Description                                                                             |
| ----------------| -----------------------------------------------------------------------------------------|
| **Static**     | This is default. Element is positioned according to the normal document flow            |
| **Relative**   | Element is positioned relative to its normal position in the document flow              |
| **Absolute**   | Element is positioned relative to the nearest positioned ancestor                       |
| **Fixed**      | Element is positioned relative to the viewport                                          |
| **Sticky**     | Element toggles between a relative and fixed position, depending on the scroll position |

Elements are then positioned to their final location with the top, bottom, left, and right properties.


### Relative Position

An element with `position: relative;` is positioned relative to its **normal position** in the document flow.

Setting the top, right, bottom, and left properties will cause the element to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.

#### Example:

```css
div.relative {
  position: relative;
  left: 30px;
}
```


### Absolute Position

An element with `position: absolute;` is positioned relative to the nearest positioned ancestor (with position other than static).

However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.

> **Note:** Absolute positioned elements are removed from the normal document flow, and can overlap other elements.

#### Example:

```css
div.relative {
  position: relative;
  width: 400px;
  height: 200px;
  border: 3px solid green;
}

div.absolute {
  position: absolute;
  top: 80px;
  right: 0;
  width: 200px;
  height: 100px;
  border: 3px solid red;
}
```

### Fixed Position

An element with `position: fixed;` is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. The top, right, bottom, and left properties are used set the final location of the element.

A fixed element does not leave a gap in the page where it would normally have been located.

This `<div>` element has position: fixed;
Notice the fixed element in the lower-right corner of the page. Here is the CSS that is used:

#### Example: 

```css
div.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 300px;
  border: 3px solid #73AD21;
}
```

### Sticky Position

An element with position: sticky; toggles between a relative and fixed position, depending on the scroll position.

A sticky element is positioned relative until a certain scroll position is reached - then it "sticks" in that place (like position:fixed).

> **Note:** You must specify at least one of the top, right, bottom or left properties, for sticky positioning to work.

#### Example:

In this example, when the sticky element reach the top of the page (top: 0), it sticks to this position

```css
div.sticky {
  position: sticky;
  top: 0;
  background-color: green;
  border: 2px solid #4CAF50;
}
```

#### Common Uses for Sticky Positioning

Sticky positioning is commonly used for:

- **Sticky headers:** Navigation bars that stick to the top when scrolling
- **Sticky sidebars:** Side content that stays visible while scrolling main content
- **Sticky table headers:** Table headers that remain visible when scrolling long tables

### Sticky vs Fixed

The key differences between **`sticky`** and **`fixed`** positioning:

| Feature           | position: sticky                | position: fixed                 |
| -------------------| ---------------------------------| ---------------------------------|
| Initial behavior  | Acts like relative              | Always fixed to viewport        |
| Space in document | Takes up space initially        | Does not take up space          |
| Scroll behavior   | Sticks after threshold          | Always fixed                    |
| Container bound   | Yes, respects parent boundaries | No, always relative to viewport |

### Important Exception

The CSS properties: `filter`, `perspective`, `transform` can also make elements positioned. They are often called "positioning contexts".

### Z Index

The `z-index` property specifies the stack order of positioned elements.

The stack order defines which element should be placed in front or behind other elements.

When elements are positioned, they can overlap other elements.

An element can have a positive or negative stack order (z-index)

#### Example:

```css
img {
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
}
```

> **Note:** `z-index` only works on positioned elements.