# CSS

CSS stands for Cascading Style Sheets

CSS is the language we use to style an HTML document.

CSS describes how HTML elements should be displayed.

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: lightblue;
}

h1 {
  color: white;
  text-align: center;
}

p {
  font-family: verdana;
  font-size: 20px;
}
</style>
</head>
<body>

<h1>CSS Example</h1>
<p>Paragraph.</p>

</body>
</html>

```

![Alt text](doc-files/c1.png)

![Alt text](doc-files/c2.png)

The selector points to the HTML element you want to style.

The declaration block contains one or more declarations separated by semicolons.

Each declaration includes a CSS property name and a value, separated by a colon.

Multiple CSS declarations are separated with semicolons, and declaration blocks are surrounded by curly braces.

```
<!DOCTYPE html>
<html>
<head>
<style>
p {
  color: cornflowerblue;
  text-align: center;
} 
</style>
</head>
<body>

<p>Paragraph</p>
<p>These paragraphs are styled with CSS.</p>

</body>
</html>
```
![Alt text](doc-files/c3.png)

`p` is a selector in CSS (it points to the HTML element you want to style: `<p>`).

`color` is a property, and `cornflowerblue` is the property value

`text-align` is a property, and `center` is the property value

## CSS Comments

A CSS comment is placed inside the `<style>` element, and starts with `/*` and ends with `*/`:

```
<!DOCTYPE html>
<html>
<head>
<style>
/* This is a single-line comment */
p {
  color: rgb(75, 75, 232);
} 
</style>
</head>
<body>

<p>This paragraph is styled with CSS.</p>
<p>CSS comments are not shown in the output.</p>

</body>
</html>
```

![Alt text](doc-files/c13.png)


Comments can be placed wherever you want in the CSS code

```
p {
  color: /*red*/blue; 
}
```
## Combination of HTML and CSS comments:

```
<!DOCTYPE html>
<html>
<head>
<style>
p {
  color: rgb(88, 131, 225); /* Set text color to blue */
}
</style>
</head>
<body>

<h2>My Heading</h2>

<!-- These paragraphs will be blue -->
<p>This paragraph is styled with CSS.</p>
<p>HTML and CSS comments are not shown in the output.</p>

</body>
</html>
```
![Alt text](doc-files/c14.png)

