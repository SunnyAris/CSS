# var()

Global variables can be accessed/used through the entire document, while local variables can be used only inside the selector where it is declared.

To create a variable with global scope, declare it inside the :root selector. The :root selector matches the document's root element.

```
:root {
  --blue: #1e90ff;
  --white: #ffffff;
}
```

To create a variable with local scope, declare it inside the selector useing the var() function that is going to use it.

```
body { background-color: var(--blue); }

h2 { border-bottom: 2px solid var(--blue); }
```

## Using Variables in Media Queries

Media Queries are about defining different style rules for different devices (screens, tablets, mobile phones, etc.).

```
@media screen and (min-width: 450px) {
  .container {
    --fontsize: 50px;
  }
   :root {
    --blue: lightblue;
  }
}
```




