# Sigma Web Development Course

## Tutorial # 15 | Inline, Internal & External CSS

[![Sigma Web Development Course - Tutorial # 15 ](https://img.youtube.com/vi/-XwZpYIyCEA/maxresdefault.jpg "Inline, Internal & External CSS")](https://www.youtube.com/watch?v=-XwZpYIyCEA&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=15)

---

## Inline, Internal & External CSS

There are 3 ways to write CSS:

1. **Inline CSS**
2. **Internal CSS**
3. **External CSS**

We will discuss what they are, when they are used and whats the recommended way of writing CSS.

---

## Inline CSS

The quick and dirty way to style an element is by using inline css. We use style attribute for add inline css.

**Example:**
```html
<h1 style="text-align: center;">Inline CSS</h1>
```

### Why this is Dirty and not Recommended 

Inline CSS makes the HTML code more longer, cluttered, repetitive, and difficult to maintain. If you want to give same styling to all the `<h1>` elements, you have to write inline CSS for every element individually unlike Internal / External CSS. Use this method sparingly.

---

## Internal CSS

The internal style is defined inside the `<style>` element, inside the head section.

**Example:**
```html
<!DOCTYPE html>
<html>
<head>
<style>
    h1 {
        color: maroon;
        margin-left: 40px;
    }
</style>
</head>
<body>
    <h1>This is a heading</h1>
</body>
</html>
```

Its useful becuase it you can write CSS directly in the HTML file without disturbing the HTML code unlike Inline CSS. Its can only be used for the HTML where its written.

> **Tip:** Use it when you want to style a single html file differently.

---

## External CSS

External CSS is an external `.css` file, as the name implies.

**Example:**
```css
body {
    text-align: center;
    text-decoration: none;
}

h1 {
    color: maroon;
    margin-left: 40px;
}
```

You have to link this `.css` file to your **HTML** file using the `<link>` element.

**Example:**
```html
<link rel="stylesheet" href="style.css">
```

This is the most recommended and used practice of writing CSS for your website. It has many advantages like you can manage all HTML files styling by linking them to a single external `.css` file making the styles reusable and centralized.

<br>

> Note: Do not add a space between the property value (20) and the unit (px):
Incorrect (space): **margin-left: 20 px;**
Correct (no space): **margin-left: 20px;**