# Borders


## `border-style`

The border-style property specifies what kind of border to display.

- `dotted` - Defines a dotted border
- `dashed` - Defines a dashed border
- `solid` - Defines a solid border
- `double` - Defines a double border
- `groove` - Defines a 3D grooved border. The effect depends on the border-color value
- `ridge` - Defines a 3D ridged border. The effect depends on the border-color value
- `inset` - Defines a 3D inset border. The effect depends on the border-color value
- `outset` - Defines a 3D outset border. The effect depends on the border-color value
- `none`- Defines no border
- `hidden` - Defines a hidden border

`border-style` property can have from one to four values (for the top border, right border, bottom border, and the left border).

```
<!DOCTYPE html>
<html>
<head>
<style>
p.dotted {border-style: dotted;}
p.dashed {border-style: dashed;}
p.solid {border-style: solid;}
p.double {border-style: double;}
p.groove {border-style: groove;}
p.ridge {border-style: ridge;}
p.inset {border-style: inset;}
p.outset {border-style: outset;}
p.none {border-style: none;}
p.hidden {border-style: hidden;}
p.mix {border-style: dotted dashed solid double;}
</style>
</head>
<body>

<h2>The border-style property</h2>
<p>This property specifies what kind of border to display:</p>

<p class="dotted">A dotted border.</p>
<p class="dashed">A dashed border.</p>
<p class="solid">A solid border.</p>
<p class="double">A double border.</p>
<p class="groove">A groove border.</p>
<p class="ridge">A ridge border.</p>
<p class="inset">An inset border.</p>
<p class="outset">An outset border.</p>
<p class="none">No border.</p>
<p class="hidden">A hidden border.</p>
<p class="mix">A mixed border.</p>

</body>
</html>
```
![Alt text](doc-files/b1.png)

## `border-width`

The width can be set as a specific size (in px, pt, cm, em, etc) or by using one of the three pre-defined values: thin, medium, or thick

```
<!DOCTYPE html>
<html>
<head>
<style>
p.a {
  border-style: solid;
  border-width: 8px;
}

p.b {
  border-style: solid;
  border-width: medium;
}

p.c {
  border-style: dotted;
  border-width: 3px;
}

p.d {
  border-style: dotted;
  border-width: thick;
}

p.e {
  border-style: double;
  border-width: 15px;
}

p.f {
  border-style: double;
  border-width: thick;
}
</style>
</head>
<body>

<h2>The border-width property</h2>
<p>This property specifies the width of the borders:</p>

<p class="a">Some text.</p>
<p class="b">Some text.</p>
<p class="c">Some text.</p>
<p class="d">Some text.</p>
<p class="e">Some text.</p>
<p class="f">Some text.</p>



</body>
</html>
```
![Alt text](doc-files/b2.png)

```
<!DOCTYPE html>
<html>
<head>
<style>
p.a {
  border-style: solid;
  border-width: 10px 30px; /* 10px top and bottom, 30px on the sides */
}

p.b {
  border-style: double;
  border-width: 20px 10px; /* 20px top and bottom, 10px on the sides */
}

p.c {
  border-style: solid;
  border-width: 20px 10px; /* 20px top and bottom, 10px on the sides */
}

p.d {
  border-style: double;
  border-width: 25px 10px 4px 35px; /* 25px top, 10px right, 4px bottom and 35px left */
}

p.e {
  border-style: solid;
  border-width: 25px 10px 4px 35px; /* 25px top, 10px right, 4px bottom and 35px left */
}
</style>
</head>
<body>

<h2>The border-width property</h2>
<p>The border-width property can have from one to four values (for the top border, right border, bottom border, and the left border):</p>

<p class="a">Some text.</p>
<p class="b">Some text.</p>
<p class="c">Some text.</p>
<p class="d">Some text.</p>
<p class="e">Some text.</p>

</body>
</html>
```
![Alt text](doc-files/b3.png)


## `border-color`

```
<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: double;
  border-color: cornflowerblue;
}

p.two {
  border-style: solid;
  border-color: darkblue;
} 

p.three {
  border-style: dotted;
  border-color: blue;
} 
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>This property specifies the color of the four borders:</p>

<p class="one">A solid red border</p>
<p class="two">A solid green border</p>
<p class="three">A dotted blue border</p>

<p><b>Note:</b> The "border-color" property does not work if it is used alone. Use the "border-style" property to set the borders first.</p>

</body>
</html>
```
![Alt text](doc-files/b4.png)

## Multicolor border

```
<!DOCTYPE html>
<html>
<head>
<style>
p.one {
  border-style: double;
  border-width: 10px;
  border-color: dodgerblue darkslateblue blue black; /* dodgerblue top, darkslateblue right, blue bottom and black left */
}
</style>
</head>
<body>

<h2>The border-color Property</h2>
<p>The border-color property can have from one to four values (for the top border, right border, bottom border, and the left border):</p>

<p class="one">A double multicolor border</p>

</body>
</html>
```
![Alt text](doc-files/b5.png)

## Individual Sides

```
<!DOCTYPE html>
<html>
<head>
<style>
p {
  border-top-style: dotted;
  border-right-style: solid;
  border-bottom-style: dotted;
  border-left-style: solid;
  border-width: 5px;
}
</style>
</head>
<body>

<h2>Individual Border Sides</h2>
<p>2 different border styles.</p>

</body>
</html>
```

## OR

```
<style>
p {
  border-style: dotted solid;
}
</style>
```

The same result

![Alt text](doc-files/b6.png)

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  text-align: center;
}
/* Four values */
p.four {
  border-style: dotted solid double dashed;
  border-width: 3px;
}

/* Three values */
p.three {
  border-style: dotted solid double;
  border-width: 3px;
}

/* Two values */
p.two {
  border-style: dotted solid;
  border-width: 3px;
}

/* One value */
p.one {
  border-style: dotted;
  border-width: 3px;
  
}
</style>
</head>
<body>

<h2>Individual Border Sides</h2>
<p class="four">4 different border styles.</p>
<p class="three">3 different border styles.</p>
<p class="two">2 different border styles.</p>
<p class="one">1 border style.</p>

</body>
</html>
```
![Alt text](doc-files/b7.png)

```
<!DOCTYPE html>
<html>
<head>
<style>
p.a {
  border: 5px solid cornflowerblue;
}

p.b {
  border-left: 6px solid cornflowerblue;
  background-color: lightcyan;
}

p.c {
  border-bottom: 6px solid cornflowerblue;
  background-color: lightcyan;
}

</style>
</head>
<body>

<h2>The border property</h2>

<p class="a">This property is a shorthand property for border-width, border-style, and border-color.</p>

<p class="b">This property is a shorthand property for border-left-width, border-left-style, and border-left-color.</p>

<p class="c">This property is a shorthand property for border-bottom-width, border-bottom-style, and border-bottom-color.</p>

</body>
</html>
```
![Alt text](doc-files/b8.png)

## Rounded Borders

```
<!DOCTYPE html>
<html>
<head>
<style>
p.normal {
  border: 2px solid cornflowerblue;
  padding: 5px;
}

p.round1 {
  border: 2px solid cornflowerblue;
  border-radius: 5px;
  padding: 5px;
}

p.round2 {
  border: 2px solid cornflowerblue;
  border-radius: 8px;
  padding: 5px;
}

p.round3 {
  border: 2px solid cornflowerblue;
  border-radius: 12px;
  padding: 5px;
}
</style>
</head>
<body>

<h2>The border-radius property</h2>
<p>This property is used to add rounded borders to an element:</p>

<p class="normal">Normal border</p>
<p class="round1">Round border</p>
<p class="round2">Rounder border</p>
<p class="round3">Roundest border</p>

</body>
</html>
```
![Alt text](doc-files/b9.png)


