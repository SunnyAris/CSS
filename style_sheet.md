# Three ways of inserting a style sheet:

- External CSS
- Internal CSS
- Inline CSS

## External CSS

### In html file

External styles are defined within the `<link>` element, inside the `<head>` section of an HTML page:


```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="style.css">
</head>
<body>

<h1>Heading</h1>
<p>Paragraph.</p>

</body>
</html>
```
### In css file

An external style sheet can be written in any text editor, and must be saved with a .css extension.

The external .css file should not contain any HTML tags.



```
body {
    background-color: rgb(140, 147, 241);
  }
  
  h1 {
    color: rgb(14, 14, 169);
    margin-left: 20px;
  }
```

![Alt text](doc-files/c10.png)

## Internal CSS

Internal styles are defined within the `<style>` element, inside the `<head>` section of an HTML page:

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: rgb(117, 140, 242);
}

h1 {
  color: rgb(93, 10, 116);
  margin-left: 40px;
} 
</style>
</head>
<body>

<h1>Heading</h1>
<p>Paragraph.</p>

</body>
</html>
```
![Alt text](doc-files/c11.png)

## Inline CSS

Inline styles are defined within the "style" attribute of the relevant element:

```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:rgb(15, 15, 224);text-align:center;">Heading</h1>
<p style="color:rgb(121, 106, 235);">Paragraph.</p>

</body>
</html>
```

![Alt text](doc-files/c12.png)

## Cascading Order

Number one has the highest priority:

1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
3. Browser default

## Multiple Style Sheets

If the internal style is defined after the link to the external style sheet, the `<h1>` elements will be "red":
```
<head>
<link rel="stylesheet" type="text/css" href="style.css">
<style>
h1 {
  color: red;
}
</style>
</head>
```

If the internal style is defined before the link to the external style sheet, the `<h1>` elements will be "blue": 

```
<head>
<style>
h1 {
  color: red;
}
</style>
<link rel="stylesheet" type="text/css" href="style.css">
</head>
```


