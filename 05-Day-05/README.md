# Sigma Web Development Course

## Tutorial # 05 | Image, Lists, and Tables in HTML

[![Sigma Web Development Course - Tutorial # 5](https://img.youtube.com/vi/1BsVhumGlNc/maxresdefault.jpg "Tutorial # 5 Image, Lists, and Tables in HTML")](https://www.youtube.com/watch?v=1BsVhumGlNc&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=5)

---

## HTML Image Tag

#### The `<img>` tag is used to show an image in your HTML page. 
The **src** attribute specifies the path to the image to be displayed:

#### Example
```bash
<img src="img_girl.jpg">
```

There are two ways to specify the URL in the src attribute:

**1. Absolute URL:** 
Links to an external image, for example:  
`src="https://images.unsplash.com/photo-1774840966298-639fb936b382".`

**2. Relative URL:**
Links to an image that is hosted within the website, for example:  
`src="image.jpg"`

### Width and Height Attributes

The `<img>` tag contain the width and height attributes, which specify the width and height of the image (in pixels):

<img src="image.jpg" width="500" height="600">

You can also set the **`width`** and **`height`** value by percentage, this percentage will be according to screen size.

For example `width="100%"` covers the entire screen.

### The alt Attribute

The **alt** attribute is an alternate text for an image, if the image for some reason cannot be displayed. This can be due to a slow connection, or an error in the src attribute. 

#### Example:  
`<img src="https://images.unsplash.com/photo-1774840966298-639fb936b382" alt="Sunset Image">`

---

## HTML Table Tag

A table in HTML consists of table cells inside rows and columns.

#### Example
A simple HTML table:

```bash
<table>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
</table>
```
#### Output 

<table>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
</table>

### Table Cells

Each table cell is defined by a `<td>` and a `</td>` tag.

> _**td** stands for table data._

### Table Rows

Each table row starts with a `<tr>` and ends with a `</tr>` tag.

> _**tr** stands for table row._

### Table Headers
If you want your cells to be table header cells. You can use the <th> tag instead of the <td> tag

> _**th** stands for table header._

---

## HTML List Tag

There are 3 types of list:

**1.** Ordered List
**2.** Unordered List
**3.** Definition Lists

### 1. Ordered List

An ordered HTML list:
```bash
<ol>
    <li>Subhan</li>
    <li>Hamza</li>
    <li>Noman</li>
    <li>Ali</li>
    <li>Usman</li>
</ol>
```

**Output:**
1. Subhan
2. Hamza
3. Noman
4. Ali
5. Usman

> _**ol** stands for **Ordered List**_
_**li** stands for **list**_

### 2. Unordered List

An unordered HTML list:
```bash
<ul>
    <li>Subhan</li>
    <li>Hamza</li>
    <li>Noman</li>
    <li>Ali</li>
    <li>Usman</li>
</ul>
```

**Output:**
- Subhan
- Hamza
- Noman
- Ali
- Usman

> _**ul** stands for **Unordered List**_
_**li** stands for **list**_

### 3. Definition Lists

A Definition List in HTML is used to represent a list of terms along with their corresponding descriptions or definitions

The `<dl>` tag defines the description list, the `<dt>` tag defines the term (name), and the `<dd>` tag describes each term.

**Example:**
```bash
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language: The standard language for creating web pages.</dd>
 
  <dt>CSS</dt>
  <dd>Cascading Style Sheets: A stylesheet language used for describing the look and formatting of a document written in HTML.</dd>
 
  <dt>JavaScript</dt>
  <dd>A programming language commonly used in web development to add interactive features.</dd>
</dl>
```

**Output:**
```
HTML
    HyperText Markup Language: The standard language for creating web pages.
    
CSS
    Cascading Style Sheets: A stylesheet language used for describing the look and formatting of a document written in HTML.

JavaScript
    A programming language commonly used in web development to add interactive features.
```