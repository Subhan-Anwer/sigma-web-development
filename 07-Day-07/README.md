# Sigma Web Development Course

## Tutorial # 07 | Forms and input tags in HTML

[![Sigma Web Development Course - Tutorial # 7](https://img.youtube.com/vi/tLBlhp0SA_0/maxresdefault.jpg "Tutorial # 7 Forms and input tags in HTML in HTML")](https://www.youtube.com/watch?v=tLBlhp0SA_0&list=PLu0W_9lII9agq7TrH9XLIKQvv0iaF2X3w&index=7)

---

## The `<form>` Tag

The HTML `<form>` tag is used to create an HTML form for user input:

```bash
<form>
.
form elements
.
</form>
```

The `<form>` element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.

---

## The `<input>` Tag

The HTML `<input>` is **most used** form element. It can be displayed in many ways, depending on the type attribute.

Here are some examples:

| Type  | Description |
| :------------- |:-------------|
| `<input type="text">`  | Displays a simple single-line text input field |
| `<input type="radio">`  | Displays a radio button (for selecting one of many choices) |
| `<input type="checkbox">`  | Displays a checkbox |
| `<input type="button">`  | Displays a clickable button |
| `<input type="submit">`  | Displays a button for submitting the form |

---

## Text Fields Attribute

The `<input type="text">` defines a simple single-line input field for **text input.**

#### Example:

```bash
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```

#### Output:

<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>

---

## The `<label>` Tag

The `<label>` tag defines a **label** for many form elements.

The `for` attribute of the `<label>` when equal to the **id attribute** of the `<input>` element, to binds together 

When the `<label>` and `<input>` binds together, user clicks the text within the `<label>` element, it toggles the radio button/checkbox, focuses on text and password fields and other input fields.

The `<label>` element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focuses on the input element.

---

## Radio Buttons

The `<input type="radio">` defines a **radio button.**

Radio buttons let a user select only **ONE** of the given number of choices.

#### Example:

```bash
<p>Choose your favorite Web language:</p>

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
```

#### Output:
Choose your favorite Web language:

<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>

---

## Checkboxes

The `<input type="checkbox">` defines a **checkbox.**

Checkboxes let a user select **ZERO or MORE** options of a given number of choices.

#### Example:

```bash
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form>
```
#### Output: 
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form>

---

## The Submit Button

The `<input type="submit">` defines a button for **submitting the form** data to a form-handler.

The **form-handler** is typically a file on the server with a script for processing input data.

The form-handler is specified in the form's **action attribute.**

#### Example:
```bash
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

#### Output:

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>

---

## The Name Attribute for `<input>`

Notice that each input field must have a `name` attribute to be submitted.

If the `name` attribute is omitted, the value of the input field will not be sent at all.

#### Example:
```bash
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" value="John"><br><br>
  <input type="submit" value="Submit">
</form>
```

#### Output: 

<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" value="John"><br><br>
  <input type="submit" value="Submit">
</form>