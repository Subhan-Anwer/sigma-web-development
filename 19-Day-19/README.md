# Sigma Web Development Course

## Tutorial # 19 | CSS Fonts, Text & Color Properties

[![Sigma Web Development Course - Tutorial # 19 ](https://img.youtube.com/vi/aFicd4-YTfo/maxresdefault.jpg "CSS Fonts, Text & Color Properties")](https://www.youtube.com/watch?v=aFicd4-YTfo&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=19)

---

## CSS Fonts

In HTML the default font is Times New Roman.
To give an element or all elements a different font in your webpage you can use the **`font-family`** CSS property.

```css
font-family: 'Poppins', Arial, Helvetica, sans-serif;
```

The first font is primary and the other fonts separated by `,` commas are fallback font, for just in case the browser of the user does not support.

### Import Fonts from Google Fonts

To use different fonts from default, use google fonts.

- Search a font. You can preview your text also with different sizing and weights.
- Get the Link Tag or @import rule of a font.
- For Link Tag add it in the head tag, where we link CSS file.
- For @import rule, add it at the top of the CSS file. 

Done now you can use your font.

**Example:**
```css
* {
    font-family: 'Poppins', sans-serif;
}
```