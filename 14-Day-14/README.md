# Sigma Web Development Course

## Tutorial # 14

[![Sigma Web Development Course - Tutorial # 14 ](https://img.youtube.com/vi/1dkfuga2_Ps/maxresdefault.jpg "Introduction to CSS")](https://www.youtube.com/watch?v=1dkfuga2_Ps&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=14)

---

## Introduction to CSS

### What is CSS?

CSS is the language we use to style a Web page.

- CSS stands for **Cascade Style Sheet.**
- CSS describes how HTML elements are to be displayed
- CSS Saves a Lot of Work!

### CSS Syntax

CSS is written a selector and a declaration block:

**Example:**
```css
h1 {
    color: blue;
    font-size: 16px;
}
```

> h1 is a selector and the key value pairs inside curly brackets `'{}'` are declation for different properties.


The selector points to the HTML element you want to style. It can be a tag like `<a>` tag or `<p>` tag and can be a class or an id.

The declaration block contains one or more declarations separated by semicolons (`;`).

Each declaration includes a CSS property **name** and a **value**, separated by a colon (`:`).

<br>

### What is a Class?

A class is an HTML attribute used for a single or group of elements to style them.

Class is reusable meaning you can give same class to multiple elements allowing them to share the same design and behavior. for example if you want to style a heading and a paragraph tag with same styling you would do it like this:
```css
h1, p {
    color: white;
    background-color: black;
}
```

By using class you can style multiple elements like `<h1>` and `<p>` by grouping them in same class like `text`:

There no rule for defining a class name, its custom not predefined however, its recommended to give a meaningful, relevant and short class name.

To select a class in CSS use dot (`.`) followed by class name in the selector.

**Example:**
```css
.text {
    color: white;
    background-color: black;
}
```

<br>

### What is an ID?

An **ID** is also an HTML attribute for elements but unlike **Class** its unique and not reusable, meaning you should different ID everytime.

Theres **no rule** for defining a ID name like class.

To select an ID for styling, use `#` followed by the ID name in selector.

**Example:**
```css
#text {
    color: white;
    background-color: black;
}
```