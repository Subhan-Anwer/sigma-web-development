# Sigma Web Development Course

## Tutorial # 25 | Styling Lists using CSS

[![Sigma Web Development Course - Tutorial # 25 ](https://img.youtube.com/vi/ZIofkptpXO8/maxresdefault.jpg "Styling Lists using CSS")](https://www.youtube.com/watch?v=ZIofkptpXO8&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=24)

---

## CSS Styling Lists

As we know in **HTML,** there are two main types of lists:

1. `<ul>` : unordered lists (list items are marked with bullets)
2. `<ol>` : ordered lists (list items are marked with numbers or letters)

**CSS** has the following properties for styling HTML lists:

- **list-style-type :** Specifies the type of list-item marker  
- **list-style-image :** Specifies an image as the list-item marker  
- **list-style-position :** Specifies the position of the list-item markers  
- **list-style :** A shorthand property for the properties above

## CSS Style List-item Markers

The CSS list-style-type property specifies the type of list-item marker in a list.

The following example shows some of the available list-item markers:

### Example

```css
ul.a {list-style-type: circle;}
ul.b {list-style-type: disc;}
ul.c {list-style-type: square;}

ol.d {list-style-type: upper-roman;}
ol.e {list-style-type: lower-roman;}
ol.f {list-style-type: lower-alpha;}
ol.g {list-style-type: decimal;}
```