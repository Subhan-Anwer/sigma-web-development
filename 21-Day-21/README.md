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

<!-- Complete this button correctly -->
<!-- <button style="padding: 10px 20px; background-color: #00ff55; color: white; border: none; cursor: pointer; color: black;" onClick="alert('The Answer is 41')">Show Answer</button> -->
<style>
    button {
        padding: 10px 20px;
        border: none;
        color: #fff;
        border-radius: 7px;
        font-weight: 700;
        transition: 0.5s ease-in-out;
        duration: 0.5s;
        transition-property: box-shadow;
        cursor: pointer;
        box-shadow: 0 0 25px rgb(5, 150, 0);
        background: none;
        color: rgb(0,220,40);
        border: 2px solid rgb(0,220,40);

    }
    button:hover {
        background: rgb(0,220,40);
        color: white;
        box-shadow: 0 0 5px rgb(0, 199, 40),
              0 0 15px rgb(0, 212, 39),
              0 0 20px rgb(0, 133, 24),
              0 0 39px rgba(0, 0, 0, 0);
}
</style>

<button onClick="alert('The Answer is 41')">Show Answer</button>
