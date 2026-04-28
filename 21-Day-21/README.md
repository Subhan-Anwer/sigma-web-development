# Sigma Web Development Course

## Tutorial # 21 | CSS Specificity & Cascade

[![Sigma Web Development Course - Tutorial # 21 ](https://img.youtube.com/vi/uTcpbPMZlFE/maxresdefault.jpg "CSS Specificity & Cascade")](https://www.youtube.com/watch?v=uTcpbPMZlFE&list=PLu0W_9lII9agq5TrH9XLIKQvv0iaF2X3w&index=21)

---

## CSS Specificity & Cascade

## Specificity Table

Following is the specificity table with most priority at the top to least priority at bottom.

| Rank | Selector                              | Example                            | Specificity |
| :--: | :------------------------------------ | :--------------------------------- | :---------- |
|  1   | Inline Styles                         | `style="color: red;"`              | 1000        |
|  2   | IDs                                   | `#header`, `#navbar`               | 100         |
|  3   | Classes, Pseudo-classes, & Attributes | `.btn`, `:hover`, `[type="text"]`  | 10          |
|  4   | Elements & Pseudo-elements            | `h1`, `div`, `::before`, `::after` | 1           |
|  5   | Universal Selector & Combinators      | `*`, `+`, `>`, `~`                 | 0           |

#### Quick Quiz

What will be the specificity value of the following selector:

```css
a.harryclass.rohan-class[href]:hover {
  color: red;
}
```
<details>
  <summary>Show Answer</summary>
    <pre>    The Answer is 41</pre>
</details>
