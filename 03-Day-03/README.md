# Sigma Web Development Course

## Tutorial # 03 | Basic Structure of an HTML Website

[![Sigma Web Development Course - Tutorial # 2](https://img.youtube.com/vi/BGeDBfCIqas/maxresdefault.jpg "Tutorial # 3 Basic Structure of an HTML Website")](https://www.youtube.com/watch?v=BGeDBfCIqas&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=3)

---

**The Basic Structure of HTML looks like this:**
```bash
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

---

In HTML a tag is a **container** to store values and other tags as well. There are two types of tags:
1. **self closing tags** 
2. **container / pair tags**

**Example of a self tag:** 
`<link rel="stylesheet" href="style.css">`

**Example of a container tag:** 
`<h1> HTML Heading Tag </h1>`

---

## HTML <!DOCTYPE> Declaration

All HTML documents must start with a `<!DOCTYPE>` declaration.

The declaration is not an HTML tag. It is an "information" to the browser about what document type to expect. All browsers support this.

In HTML 5, the declaration is simple:

```
<!DOCTYPE html>
```

---

## HTML `<html>` Tag

The `<html>` tag represents the root of an HTML document.

The `<html>` tag is the container for all other HTML elements (except for the `<!DOCTYPE>` tag).

> **📝 Note:** You should always include the lang attribute inside the <html> tag, to declare the language of the Web page. This is meant to assist search engines and browsers.

---

## HTML `<head>` Tag

It is the container for all metadata (data about data). It is the **Child Tag** of `<html>` tag and sibling of the `<body>` tag. Metadata is data about the HTML document. Metadata is not displayed.

---

### HTML `<body>` Tag

The <body> tag defines the document's body. This is what you see on the **website's interface.** It contains all the contents of an HTML document, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.

> **📝 Note:** There can only be one <body> element in an HTML document.