# Sigma Web Development Course

## Tutorial # 22 | CSS Sizing Units

[![Sigma Web Development Course - Tutorial # 22 ](https://img.youtube.com/vi/nkaAJYfRDVk/maxresdefault.jpg "CSS Sizing Units")](https://www.youtube.com/watch?v=nkaAJYfRDVk&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=22)

---

## CSS Sizing Units

There are many different CSS sizing units that can be used to specify the length / size of elements on a webpage. Some of the most common units are discussed below.

### Pixel (px)

The pixel is a fixed unit of measurement that represents a single dot on the screen. It is commonly used for precise control over the size of elements, such as buttons, images and text.

```css
.element {
  width: 200px;
  height: 100px;
}
```

### Viewport Width (vw)

Viewport Width is used for responsive design and is based on the width of the viewport (screen). 

**`1vw`** is equal to `1%` of the viewport width. This unit allows elements to scale proportionally to the size of the viewport.

```css
.element {
  width: 50vw; /* This will make the element take up 50% of the viewport width */
}
```

### Viewport Height (vh)

Viewport Height is as you have guessed the height of the screen or viewport. 

**`1vh`** is equal to `1%` of the viewport height. This unit allows elements to scale proportionally to the size of the viewport.

### EM (em)

In CSS the child element inherits some properties from the parent element. The `em` unit is a relative unit to its parent.

For instance, if we make a parent element name `container` and set its font size to 16px, then the child element will inherit this font size. If we set the child element's font size to 1.5em, it will be 1.5 times the font size of the parent element, which is 24px (16px * 1.5).

```css
.container {
  font-size: 16px;
}

.child {
  font-size: 1.5em; /* This will be 24px (16px * 1.5) */
}
```

#### When its useful?

The `em` unit is particularly useful for creating scalable and responsive designs.

For Example you create a text blog page. You set the container font size to 10px and want other text elements to scale relative to it.

You can set the heading size to 3em, which means it will be 1.5 times (30px) the font size of the container. Secondary heading size to 2em (20px) and paragraph element to 1.5em (15px).

You made buttons for small, standarad, large text size, you can just change the container font size to 12px and all the text elements will scale accordingly, making it easy to maintain a consistent design across different screen sizes and devices.

### REM (rem)

The `rem` unit is similar to `em`, but it is relative to the root element (usually the `<html>` element) rather than the parent element. This means that all elements using `rem` will be based on the same root font size.

In other words, the primary difference between `em` and `rem` is the **reference point** used to calculate their size.

> Note: REM (`rem`) and EM (`em`) can be used for other sizing properties such as width & height not just font size. 

### Viewport Minimum (vmin)

Viewport Minimum is `1%` of the smallest dimension of the viewport (either width or height).

For example, if the viewport is of PC with 1200px width and  800px height, then the `vmin` will be based on the height (800px) and 1vmin will be equal to 8px. And Opposite on mobile where the vmin is based on the width as mobile screens are usually taller than they are wider.

### Viewport Maximum (vmax)

Viewport Maximum is exactly opposite of the Viewport Minimum, it is `1%` of the biggest dimension of the viewport.

---

### Conclusion

These are **not** the only CSS sizing units but these are the most commonly used ones. Each unit has its own use case. What matters is to understand the use case of each unit and use them accordingly and efficiently to create responsive and scalable designs.

