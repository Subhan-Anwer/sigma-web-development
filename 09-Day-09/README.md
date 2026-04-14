# Sigma Web Development Course

## Tutorial # 09 | Id & Classes in HTML

[![Sigma Web Development Course - Tutorial # 9](https://img.youtube.com/vi/vlAWzsGd-Yk/maxresdefault.jpg "Tutorial # 9 Id & Classes in HTML")](https://www.youtube.com/watch?v=vlAWzsGd-Yk&list=PLu0W_9lII9agq9TrH9XLIKQvv0iaF2X3w&index=9)

---

## ID in HTML

#### What is ID?
**Id** is an attribute of a HTML element. An element cannot have multiple ID's and same ID as another element.

#### How to give ID to an Element
Use `id="value"` to give ID an element in HTML.

**Example:**

```bash
<h1 id="heading">Heading</h1>
```

#### How to Select ID and give Styling in CSS 

In CSS file, Use dot `.` followed by ID e.g: `heading`, open parenthesis (curly brackets). Write the properties and their value in the parenthesis e.g: `property: value;`

**Example:**
```bash
.heading {
    color: red;
}
```

---

## Class in HTML

#### What is Class?
A **class** is also an attribute of a HTML element but unlike **ID** an element can have multiple classes and multiple elements can have same class.

#### How to give Class to an Element
Use `class="value"` to give class an element in HTML.

**Example:**

```bash
<h1 class="bg-grey">Heading</h1>
```

#### How to Select Class and give Styling in CSS

In CSS file, Use dot `#` followed by Class e.g: `bg-yellow`, open parenthesis (curly brackets). Write the properties and their value in the parenthesis e.g: `property: value;`

**Example:**
```bash
.bg-yellow {
    background-color: yellow;
}
```

> **Note:** for selecting ID we use **#** and for selecting Class we use **.** dot