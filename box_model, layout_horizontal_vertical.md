# Box model

CSS box model is essentially a box that wraps around every HTML element. It consists of: content, padding, borders and margins

![Alt text](doc-files/bm1.png)

- Content - The content of the box, where text and images appear

- Padding - Clears an area around the content. The padding is transparent

- Border - A border that goes around the padding and content

- Margin - Clears an area outside the border. The margin is transparent


```
<!DOCTYPE html>
<html>
<head>
<style>
div {
  background-color: rgb(142, 187, 235);
  width: 300px;
  border: 25px solid rgb(95, 82, 237);
  padding: 30px;
  margin: 20px;
}
</style>
</head>
<body>

<h2>Box Model</h2>

<p>The CSS box model is essentially a box that wraps around every HTML element. It consists of: borders, padding, margins, and the actual content.</p>

<div>This text is the content of the box add a 30px padding, 20px margin and a 25px blue border.</div>

</body>
</html>
```

![Alt text](doc-files/bm2.png)

```
<!DOCTYPE html>
<html>
<head>
<style>
div {
  width: 230px;
  height: 70px;
  padding: 10px;
  border: 5px solid gray;
  margin: 0px;
}
img {
  border: 5px solid gray;
}
</style>
</head>
<body>

<h2>Calculate the total width:</h2>

<img src="doc-files/chibi2.jpg" width="250" height="250" alt="chibi">
<div>The picture above is 250px wide. The total width of this element is also 250px. The total height of this element is 70px.</div>

</body>
</html>
```
![Alt text](doc-files/bm3.png)
```
230px (width of content area)
+ 20px (left padding + right padding)
+ 10px (left border + right border)
= 250px (total width)

  70px (height of content area)
+ 20px (top padding + bottom padding)
+ 10px (top border + bottom border)
= 100px (total height)
```

# Center Align Elements

```
<!DOCTYPE html>
<html>
<head>
<style>
.center {
  margin: auto;
  width: 60%;
  border: 3px solid orange;
  padding: 10px;
}
</style>
</head>
<body>

<h2>Center Align Elements</h2>
<p> margin: auto - horizontally center a block element (like div);</p>

<div class="center">
  <p>Center</p>
</div>

</body>
</html>
```

![Alt text](doc-files/lh1.png)

```
<!DOCTYPE html>
<html>
<head>
<style>
.center {
  text-align: center;
  border: 3px solid orange;
}
</style>
</head>
<body>

<h2>Center Text</h2>

<div class="center">
  <p>Center</p>
</div>

</body>
</html>
```

![Alt text](doc-files/lh2.png)


```
<!DOCTYPE html>
<html>
<head>
<style>
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
</head>
<body>

<h2>Center an image</h2>
<p>Center image - set left and right margin to auto, and make it into a block element.</p>

<img src="doc-files/chibi2.jpg" alt="chibi" style="width:40%">

</body>
</html>
```

![Alt text](doc-files/lh3.png)


```
<!DOCTYPE html>
<html>
<head>
<style>
.right {
  position: absolute;
  right: 0px;
  width: 300px;
  border: 3px solid orange;
  padding: 10px;
}
</style>
</head>
<body>

<h2>Right align with the position property</h2>

<p>Right align elements with the position property:</p>

<div class="right">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...</p>
</div>

</body>
</html>
```
![Alt text](doc-files/lh5.png)

```
<!DOCTYPE html>
<html>
<head>
<style>
.right {
  float: right;
  width: 300px;
  border: 3px solid orange;
  padding: 10px;
}
</style>
</head>
<body>

<h2>Right align with the float property</h2>

<p>Right align elements with the float property:</p>

<div class="right">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...</p>
</div>

</body>
</html>
```
![Alt text](doc-files/lh6.png)

```
<!DOCTYPE html>
<html>
<head>
<style>
.center {
  padding: 70px 0;
  border: 3px solid orange;
}
</style>
</head>
<body>

<h2>Center vertically with padding</h2>

<p>Padding property to center the div element vertically:</p>

<div class="center">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...</p>
</div>

</body>
</html>
```
![Alt text](doc-files/lh7.png)


```
<!DOCTYPE html>
<html>
<head>
<style>
.center {
  padding: 70px 0;
  border: 3px solid orange;
  text-align: center;
}
</style>
</head>
<body>

<h2>Center with padding and text-align</h2>

<p>Padding and text-align to center the div element both vertically and horizontally:</p>

<div class="center">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet...</p>
</div>

</body>
</html>
```
![Alt text](doc-files/lh8.png)



