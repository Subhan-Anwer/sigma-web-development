# Sigma Web Development Course

## Tutorial # 24 | CSS Shadows and Outlines

[![Sigma Web Development Course - Tutorial # 24 ](https://img.youtube.com/vi/BZJcNU648Tc/maxresdefault.jpg "CSS Shadows and Outlines")](https://www.youtube.com/watch?v=BZJcNU648Tc&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=24)

---

## Box Shadow

**Box shadow** is a CSS property used to add shadow effect to an element. It can be used for any element whether it is a div, span, image, etc.

### Syntax

```css
box-shadow: offset-x offset-y blur-radius spread-radius color inset;
```

- **offset-x**: Horizontal distance of the shadow. Positive values shift shadows right; negative values shift left.
- **offset-y**: Vertical distance of the shadow. Positive values shift shadows down; negative values shift up.
- **blur-radius**: Blur radius of the shadow. Higher value means more blur
- **spread-radius**: Spread radius of the shadow. Higher value means more spread
- **color**: Color of the shadow.
- **inset**: Inset shadow. It is optional, By default it is outset.

### Example

```css
.box-shadow { box-shadow: 10px 10px 15px #888888; }
```

---

## Text Shadow

The CSS text-shadow property applies a shadow to text. In simple form, you only specify the horizontal and vertical shadow.

### Example

```css
h1 { text-shadow: 2px 2px; }
```

In addition, you can add a shadow color and blur effect.

### Example

```css
h1 { text-shadow: 2px 2px 5px red; }
```

### Example Output
<style>
h2.text-shadow {
  text-shadow: 2px 2px 5px red;
}
</style>
<h2 class="text-shadow">
Text Shadow Preview
</h2>

---

## CSS Outline

An outline is a line that is drawn around elements, **OUTSIDE** the borders, to make the element "stand out".

### Syntax

```css
.element { outline: width style color; }
```

### Example

```css
.element { outline: #4CAF50 solid 10px; }
```

### Example Output
<br>
<style>
h5 {
  border: 2px solid black;
  outline: #1b8a1fff solid 10px;
  margin: auto;  
  padding: 20px;
  text-align: center;
}
</style>
<h5>This element has a 2px black border and a green outline with a width of 10px.</h5>

<br><br>

> **Note:** Outline differs from borders! The outline is drawn outside the element's border, and may overlap other content. Also, the outline is NOT a part of the element's dimensions; the element's total width and height is not affected by the width of the outline.

### Outline-Style Property

he [outline-style](#css-outline) property specifies the style of the outline, and can have one of the following values:

| Style  | Description                  |
| :-------| :-----------------------------|
| dotted | Defines a dotted outline.    |
| dashed | Defines a dashed outline.    |
| solid  | Defines a solid outline.     |
| double | Defines a double outline.    |
| groove | Defines a 3D-groove outline. |
| ridge  | Defines a 3D-ridge outline.  |
| inset  | Defines a 3D-inset outline.  |
| outset | Defines a 3D-outset outline. |
| none   | Defines no outline, Default. |
| hidden | Defines a hidden outline.    |

### Example

```css
p.dotted {outline-style: dotted;}
p.dashed {outline-style: dashed;}
p.solid {outline-style: solid;}
p.double {outline-style: double;}
p.groove {outline-style: groove;}
p.ridge {outline-style: ridge;}
p.inset {outline-style: inset;}
p.outset {outline-style: outset;}
```

### Example Output
<style>
h4 {
    outline: #1b8a1fff 2px;
    padding: 10px;
    text-align: center;
}
h4.dotted {outline-style: dotted;}
h4.dashed {outline-style: dashed;}
h4.solid {outline-style: solid;}
h4.double {outline-style: double;}
h4.groove {outline-style: groove;}
h4.ridge {outline-style: ridge;}
h4.inset {outline-style: inset;}
h4.outset {outline-style: outset;}
</style>
<h4 class="dotted">A dotted outline.</h4>
<h4 class="dashed">A dashed outline.</h4>
<h4 class="solid">A solid outline.</h4>
<h4 class="double">A double outline.</h4>
<h4 class="groove">A groove outline.</h4>
<h4 class="ridge">A ridge outline.</h4>
<h4 class="inset">An inset outline.</h4>
<h4 class="outset">An outset outline.</h4>