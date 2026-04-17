# Sigma Web Development Course

## Tutorial # 13 | Exercise 1 - Entities, Code & More Miscellaneous Tags

[![Sigma Web Development Course - Tutorial # 13 ](https://img.youtube.com/vi/cvsbHZcDx8w/maxresdefault.jpg "Exercise 1 - Entities, Code & More Miscellaneous Tags")](https://www.youtube.com/watch?v=cvsbHZcDx8w&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=13)

---

## Entities in HTML

### What Are HTML Entities?

HTML Eentities are used to display special characters that are reserved in HTML by representing them in a format that the browser can understand.

They start with an ampersand (`&`) and end with a semicolon (`;`).

<br>

### Why Use HTML Entities?

Lets understand it with some example.

Try to write & display the sign of `<p>` inside any tag like heading or paragraph. You will see that it wont appear because the HTML will understand it as a tag. If you want to actually display the tag, thats where you will use the HTML Entities.

<br>

### When To Use HTML Entities?

- **Reserved Characters:** Characters like `<`, `>`, and `&` are reserved in HTML.
- **Special Symbols:** For symbols like `©`, `®`, or mathematical symbols.
- **Non-Breaking Spaces:** To create white spaces that won't break into a new line.

<br>

### Types Of Entities In HTML

There are two types of entities in HTML, **Entity Names** and **Entity Numbers**

Entity names look like this: *`&entity_name;`*
Entity numbers look like this: *`&#entity_number;`*

> Entity names are easier to remember than entity numbers as they are the short form of their character's purpose. 

<br>

### Common HTML Entities

```bash
&lt;  for <
&gt;  for >
&amp; for &
&nbsp; for a non-breaking space
&copy; for ©
```

<br>

### Example Of Using HTML Entities

Entities can be implemented easily within HTML code. Here are some examples:

#### Using Reserved Characters
```bash
<p>The price is 10 &lt; 20.</p>
```

#### Displaying Special Symbols
```bash
<p>Copyright &copy; 2023.</p>
```

#### Creating Non-Breaking Spaces
```bash
<p>This is an example&nbsp;text.</p>
```

### Conclusion

HTML entities are essential for rendering special or reserved characters on a web page. Understanding how to use them effectively is key to creating web pages that display content as intended.

<br>

---

<br>

## Pre Tags

The `<pre>` tag defines preformatted text.
In HTML all new lines are ignored and all white spaces between text are count as one. If you literally want to add the new line or white spaces, you can use `<pre>` tag.

**Example:**
```bash
<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks
</pre>
```

**Output:**

<pre>
Text in a pre element
is displayed in a fixed-width
'font', and it preserves
both      spaces and
line breaks
</pre>

<br>

---

<br>

## Quotation Tag

Quotation tag is used when you want to define content (text) that is taken from another source. for example a using the content from a Blog Post or talking about the headline from the News Article.

### How To Use Quotation Tag

There are two types of Quotation Tag:

- **`<blockquote>` :** used for longer quotations or multiline quotations.
- **`<q>` :** used for short quotations or inline / single line quotations.

### Examples:

#### 1. Short Inline Quote (`<q>`)

Use this when you want to mention a quote as part of a regular sentence.

```bash
<p>As Albert Einstein once said, <q cite="https://example.com">Imagination is more important than knowledge.</q></p>
```

**Result:** The browser will automatically wrap the text in double quotes.

<br>

#### 2. Long Block Quote (`<blockquote>`)

```bash
<blockquote cite="https://worldwildlife.org">
  <p>For 50 years, WWF has been protecting the future of nature. The world's leading conservation organization, WWF works in 100 countries and is supported by 1.2 million members.</p>
</blockquote>
```

> **Note:** Both tags support cite attribute, it is used to pass the source url of the quotation.

<br>

### Why Use These Tags?

You will think that why cant i just type this normally, if for styling i can use span tag, the answer is Yes you can. But its very important for **SEO**. 

Search Engine use these tags to understand the context and original source of your content, and establish your credibility not assuming you copied someone else's content and hence indexing your page better and making it rank.

In short these tags provide semantic meaning to your page and content and telling search engine that you used this quotation from this source. 