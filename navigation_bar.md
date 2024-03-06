# Navigation Bar

```
<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

li a {
  display: block;
  width: 60px;
  background-color: #e6de0c;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<p>Whole link area is clickable, not just the text.</p>

</body>
</html>
```
![Alt text](doc-files/nb1.png)

```
<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #efeef3;
}

li a {
  display: block;
  color: #3719f7;
  padding: 8px 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #5f91ed;
  color: white;
}
</style>
</head>
<body>

<h2>Vertical Navigation Bar</h2>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
```
![Alt text](doc-files/nb2.png)

# Active/Current Navigation Link

```
<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #efeef3;
}

li a {
  display: block;
  color: #3719f7;
  padding: 8px 16px;
  text-decoration: none;
}

li a.active {
  background-color: #5f91ed;
  color: white;
}

li a:hover:not(.active) {
  background-color: #8e9ace;
  color: white;
}

</style>
</head>
<body>

<h2>Vertical Navigation Bar</h2>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
```
![Alt text](doc-files/nb3.png)

# Center Links & Add Borders

```
<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #efeef3;
  border: 1px solid #3d08ed;
}

li a {
  display: block;
  color: #3719f7;
  padding: 8px 16px;
  text-decoration: none;
}

li {
  text-align: center;
  border-bottom: 1px solid #3d08ed;
}

li:last-child {
  border-bottom: none;
}

li a.active {
  background-color: #5f91ed;
  color: white;
}

li a:hover:not(.active) {
  background-color: #8e9ace;
  color: white;
}

</style>
</head>
<body>

<h2>Vertical Navigation Bar</h2>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
```
![Alt text](doc-files/nb4.png)

# Full-height Fixed Vertical Navbar

```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  margin: 0;
  background-color: #b9caff;
}
h2 {
    color: rgb(14, 14, 169);
    margin-left: 20px;
  }

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 25%;
  background-color: #b9caff;
  position: fixed;
  height: 100%;
  overflow: auto;
}

li a {
  display: block;
  color: #380fec;
  padding: 8px 16px;
  text-decoration: none;
}

li a.active {
  background-color: #3350f3;
  color: white;
}

li a:hover:not(.active) {
  background-color: #8991ee;
  color: white;
}
</style>
</head>
<body>

<ul>
  <li><a class="active" href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

<div style="margin-left:25%;padding:1px 16px;height:1000px;">
  <h2>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Adipiscing enim eu turpis egestas pretium aenean pharetra magna. Consequat id porta nibh venenatis cras sed. Purus in massa tempor nec. Sed libero enim sed faucibus. Habitant morbi tristique senectus et netus et malesuada fames ac. Felis eget nunc lobortis mattis aliquam faucibus purus. Tellus cras adipiscing enim eu turpis. Sollicitudin nibh sit amet commodo. Cras semper auctor neque vitae.

    Elementum curabitur vitae nunc sed velit dignissim sodales ut eu. Etiam erat velit scelerisque in. Porttitor lacus luctus accumsan tortor posuere. Integer malesuada nunc vel risus commodo viverra maecenas accumsan lacus. Maecenas volutpat blandit aliquam etiam. Bibendum ut tristique et egestas quis ipsum suspendisse ultrices. Neque volutpat ac tincidunt vitae semper. Felis imperdiet proin fermentum leo vel orci porta non. Platea dictumst quisque sagittis purus sit amet volutpat consequat mauris. Est velit egestas dui id ornare arcu odio ut. Gravida arcu ac tortor dignissim convallis aenean et tortor at. Urna id volutpat lacus laoreet non curabitur. Nisl tincidunt eget nullam non nisi est sit amet. Tristique magna sit amet purus. Pulvinar proin gravida hendrerit lectus a. Eu sem integer vitae justo eget magna fermentum. Scelerisque mauris pellentesque pulvinar pellentesque habitant morbi tristique senectus. Massa tempor nec feugiat nisl pretium fusce id velit ut. Facilisis mauris sit amet massa vitae tortor.</h2>
 
</div>

</body>
</html>
```

![Alt text](doc-files/nb5.png)

# Horizontal Navigation Bar

```
<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #dddddd;
}

li {
  float: left;
}

li a {
  display: block;
  padding: 8px;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
```
![Alt text](doc-files/nb6.png)

```
<!DOCTYPE html>
<html>
<head>
<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
}

li {
  float: left;
}

li a {
  display: block;
  padding: 8px;
  background-color: #dddddd;
}
</style>
</head>
<body>

<ul>
  <li><a href="#home">Home</a></li>
  <li><a href="#news">News</a></li>
  <li><a href="#contact">Contact</a></li>
  <li><a href="#about">About</a></li>
</ul>

</body>
</html>
```
![Alt text](doc-files/nb7.png)





