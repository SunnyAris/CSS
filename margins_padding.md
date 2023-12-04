# Margins

CSS has properties for specifying the margin for each side of an element:

- margin-top
- margin-right
- margin-bottom
- margin-left

All the margin properties can have the following values:

- auto - the browser calculates the margin
- length - specifies a margin in px, pt, cm, etc.
- % - specifies a margin in % of the width of the containing element
- inherit - specifies that the margin should be inherited from the parent element




```
<!DOCTYPE html>
<html>
<head>
<style>
div {
  margin: 50px;
  border: 5px solid #4c61af;
}
</style>
</head>
<body>

<h2>CSS Margins</h2>

<div>This element has a margin of 50px.</div>

</body>
</html>
```
![Alt text](doc-files/b10.png)


```
<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 5px solid black;
  margin-top: 20px;
  margin-bottom: 20px;
  margin-right: 50px;
  margin-left: 50px;
  background-color: cornflowerblue;
}
</style>
</head>
<body>

<h2>Using individual margin properties</h2>

<div>This div element has a top margin of 20px, a right margin of 50px, a bottom margin of 20px, and a left margin of 50px.</div>

</body>
</html>
```

![Alt text](doc-files/b11.png)

## Shorthand Property

The margin property is a shorthand property for the following individual margin properties:

- margin-top
- margin-right
- margin-bottom
- margin-left

So, here is how it works:

If the margin property has four values:

### margin: 25px 50px 75px 100px;
- top margin is 25px
- right margin is 50px
- bottom margin is 75px
- left margin is 100px

```
<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 1px solid black;
  margin: 25px 50px 75px 100px;
  background-color: cornflowerblue;
}
</style>
</head>
<body>

<h2>The margin shorthand property - 4 values</h2>

<div>This div element has a top margin of 25px, a right margin of 50px, a bottom margin of 75px, and a left margin of 100px.</div>

<hr>

</body>
</html>

```

![Alt text](doc-files/b12.png)


### margin: 25px 50px 75px;
- top margin is 25px
- right and left margins are 50px
- bottom margin is 75px

```
p {
  margin: 25px 50px 75px;
}
```

### margin: 25px 50px;
- top and bottom margins are 25px
- right and left margins are 50px

```
p {
  margin: 25px 50px;
}
```

### margin: 25px;
- all four margins are 25px

```
p {
  margin: 25px;
}
```

## `margin: auto`

```
<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 350px;
  margin: auto;
  border: 5px solid cornflowerblue;
}
</style>
</head>
<body>

<h2>Use of margin: auto</h2>
<p>Set the margin property to auto to horizontally center the element within its container. The element will then take up the specified width, and the remaining space will be split equally between the left and right margins:</p>

<div>
This div will be horizontally centered because it has margin: auto;
</div>

</body>
</html>
```
![Alt text](doc-files/b13.png)

## `inherit` value

```
<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 5px solid cornflowerblue;
  margin-left: 50px;
}

p.ex1 {
  margin-left: inherit;
}
</style>
</head>
<body>

<h2>Use of the inherit value</h2>
<p>Let the left margin be inherited from the parent element:</p>

<div>
<p class="ex1">This paragraph has an inherited left margin (from the div element).</p>
</div>

</body>
</html>
```
![Alt text](doc-files/b14.png)


## Margin Collapse

Top and bottom margins of elements are sometimes collapsed into a single margin that is equal to the largest of the two margins.

This does not happen on left and right margins. Only top and bottom margins.

```
<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  margin: 0 0 50px 0;
}

h2 {
  margin: 20px 0 0 0;
}
</style>
</head>
<body>

<p>In this example the h1 element has a bottom margin of 50px and the h2 element has a top margin of 20px. So, the vertical margin between h1 and h2 should have been 70px (50px + 20px). However, due to margin collapse, the actual margin ends up being 50px.</p>

<h1>Heading 1</h1>
<h2>Heading 2</h2>

</body>
</html>
```

# Padding

Padding is used to create space around an element's content, inside of any defined borders.

```
<!DOCTYPE html>
<html>
<head>
<style>
div {
  padding: 50px;
  border: 5px solid #4c5baf;
}
</style>
</head>
<body>

<h2>CSS Padding</h2>
<div>This element has a padding of 50px.</div>

</body>
</html>
```
![Alt text](doc-files/p1.png)

## Individual Sides

CSS has properties for specifying the padding for each side of an element:

- padding-top
- padding-right
- padding-bottom
- padding-left

All the padding properties can have the following values:

- length - specifies a padding in px, pt, cm, etc.
- % - specifies a padding in % of the width of the containing element
- inherit - specifies that the padding should be inherited from the parent element

```
<!DOCTYPE html>
<html>
<head>
<style>
div {
  border: 5px solid black;
  background-color: cornflowerblue;
  padding-top: 3cm;
  padding-right: 3cm;
  padding-bottom: 3cm;
  padding-left: 3cm;
}
</style>
</head>
<body>
<h2>Using individual padding properties</h2>

<div>This div element has a top padding of 3cm, a right padding of 3cm, a bottom padding of 3cm, and a left padding of 3cm.</div>
</html>
```

![Alt text](doc-files/p2.png)


## Padding - Shorthand Property 

The padding property is a shorthand property for the following individual padding properties:

- padding-top
- padding-right
- padding-bottom
- padding-left

If the padding property has four values:

 padding: 25px 50px 75px 100px;
- top padding is 25px
- right padding is 50px
- bottom padding is 75px
- left padding is 100px

Padding property values for three, two and one is almost the same as margins property.

## Padding and Element Width

 `<div>` element is given a width of 100px. However, the actual width of the `<div>` element will be 150px (100px + 25px of left padding + 25px of right padding):

```
<!DOCTYPE html>
<html>
<head>
<style>
div.ex1 {
  width: 100px;
  background-color: rgb(92, 162, 216);
}

div.ex2 {
  width: 100px;
  padding: 25px;
  background-color: rgb(83, 194, 231);
}

div.ex3 {
  margin: 100px;
  border: 5px solid #4c61af;
}
</style>
</head>
<body>

<h2>Padding and element width</h2>

<div class="ex1">This div is 100px wide.</div>
<br>

<div class="ex2">Padding. The width of this div is 150px, even though it is defined as 100px in the CSS.</div>
<br>
<div class="ex3">Margin. The width of this div is 100px</div>
</body>
</html>
```

![Alt text](doc-files/p3.png)

```
<!DOCTYPE html>
<html>
<head>
<style>
div.ex1 {
  width: 100px;
  background-color: rgb(73, 160, 221);
}

div.ex2 {
  width: 100px;
  padding: 25px;
  box-sizing: border-box;
  background-color: rgb(62, 187, 229);
}
</style>
</head>
<body>

<h2>Padding and element width - with box-sizing</h2>

<div class="ex1">This div is 100px wide.</div>
<br>

<div class="ex2">The width of this div remains at 100px, in spite of the 50px of total left and right padding, because of the box-sizing: border-box property.
</div>

</body>
</html>
```
![Alt text](doc-files/p4.png)

