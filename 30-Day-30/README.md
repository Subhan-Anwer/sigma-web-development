# Sigma Web Development Course

## Tutorial # 30 | Exercise 3

[![Sigma Web Development Course - Tutorial # 30 - CSS Variables ](https://img.youtube.com/vi/ovRU9xHfly4/maxresdefault.jpg "CSS Variables")](https://www.youtube.com/watch?v=ovRU9xHfly4&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=30)

---

## CSS Variables

Variable in CSS are used like the same way as variables in programming languages. They are used to store values that can be reused throughout the CSS file. This makes it easier to maintain and update styles, as you only need to change the value in one place instead of copy & pasting for every element.

CSS variables have access to the DOM, which means that you can create variables with local or global scope, change the variables with JavaScript, and change the variables based on media queries.

But Declaring and using them in CSS is a bit different because CSS is not a programming language. 

### Declaring CSS Variables

A CSS variable name must begin with two dashes (--) and is case sensitive! CSS variables can have a global or local scope.

##### Global CSS Variables

Global variables can be accessed through the entire document, while local variables can be used only inside the selector where it is declared.

To create a global variable, declare it inside the :root selector. The :root selector matches the document's root element.

**Syntax Example:**

```css
:root {
    --primary-color: #3498db;
    --secondary-color: #2ecc71;
    --font-size: 16px;
}
```

##### Local CSS Variables

To create a local variable, declare it inside the selector that is going to use it. It will override the global variable if it has the same name.

A local variable can be accessed only inside the selector where it is declared.

**Syntax Example:**

```css
.container {
    --primary-color: #3498db;
}
```

### Accessing CSS Variables

To access a CSS variable, use the var() function. The **var()** function denotes **'variable'** and is used to insert a custom/predefined variable.

**Syntax Example:**

```css
.container {
    background-color: var(--primary-color);
}
```

### Fallback Values

What if the variable you are trying to use is not defined? In that case, you can also set a fallback value. The fallback value will be used if the variable is not defined. Its totally optional.

**Syntax Example:**

```css
.container {
    background-color: var(--primary-color, #0d65a0);
}
```