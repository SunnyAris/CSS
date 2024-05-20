## Styling Forms

Attribute selectors used for styling forms without class or ID

```
<!DOCTYPE html>
<html>
<head>
<style>
input[type="text"] {
  width: 150px;
  display: block;
  margin-bottom: 10px;
  background-color: gold;
  color: black;
}

input[type="button"] {
  width: 120px;
  margin-left: 35px;
  display: block;
}
</style>
</head>
<body>

<h2>Styling Forms</h2>

<form name="input" action="" method="get">
  Firstname:<input type="text" name="Name" value="Sunny" size="20">
  Lastname:<input type="text" name="Name" value="Aris" size="20">
  <input type="button" value="Example Button">
</form>

</body>
</html>
```
![Alt text](doc-files/sl20.png)

## Full width input field

```
<!DOCTYPE html>
<html>
<head>
<style> 
input {
  width: 100%;
}
</style>
</head>
<body>

<h2>A full width input field</h2>

<form>
  <label for="fname">Name</label>
  <input type="text" id="fname" name="fname">
</form>

</body>
</html>
```
![Alt text](doc-files/sf.png)

## Padded input fields

```
<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 20px 0;
  box-sizing: border-box;
  border-style: double;
  border-color: dodgerblue;
  border-width: 10px;
}
</style>
</head>
<body>

<h2>Padded input fields with borders</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname">
</form>

</body>
</html>
```
![Alt text](doc-files/sf1.png)

## Input fields with color 

```
<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 5px solid #ece51f;
  outline: none;
}

input[type=text]:focus {
  background-color: cornflowerblue;
}
</style>
</head>
<body>

<h2>Input fields with color on :focus</h2>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname" value="Sunny">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname" value="Aris">
</form>

</body>
</html>
```
![Alt text](doc-files/sf2.png)

## Input fields with yellow border on :focus

```
<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 3px solid #c9c9c9;
  -webkit-transition: 5s;
  transition: 5s;
  outline: none;
}

input[type=text]:focus {
  border: 3px solid #fbe32c;
}
</style>
</head>
<body>

<h2>Input fields with yellow border on :focus</h2>

<p>Yellow border color when it gets focus. Property is animated to change the border color (takes 5 seconds to change the color on focus):</p>

<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname" value="Sunny">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname" value="Aris">
</form>

</body>
</html>
```

![Alt text](doc-files/sf3.png)

```
<!DOCTYPE html>
<html>
<head>
<style> 
input[type=text] {
  width: 100%;
  box-sizing: border-box;
  border: 2px solid #ccc;
  border-radius: 4px;
  font-size: 16px;
  background-color: white;
  background-image: url('doc-files/searchicon.png'); 
  background-size: 25px;
  background-position: 10px 10px; 
  background-repeat: no-repeat;
  padding: 12px 20px 12px 40px;
}
</style>
</head>
<body>

<h2>Input field with an icon inside</h2>

<form>
  <input type="text" name="search" placeholder="Search.."> 
</form>

</body>
</html>
```

![Alt text](doc-files/sf4.png)

## Styling Textareas

```
<!DOCTYPE html>
<html>
<head>
<style> 
textarea {
  width: 100%;
  height: 150px;
  padding: 12px 20px;
  box-sizing: border-box;
  border: 14px double #aad7f6;
  border-radius: 44px;
  background-color: #c0e3fd;
  font-size: 16px;
  resize: none;
  outline-color: #355ce8;
}
</style>
</head>
<body>

<h2>Styling textarea</h2>

<form>
  <textarea>Some text...</textarea>
</form>

</body>
</html>
```
![Alt text](doc-files/sf6.png)

## Styling a select menu

```
<!DOCTYPE html>
<html>
<head>
<style> 
select {
  width: 100%;
  padding: 16px 20px;
  border: none;
  border-radius: 4px;
  background-color: #a0c9f7;
  outline-color: #03165a;
}
</style>
</head>
<body>

<h2>Styling a select menu</h2>

<form>
  <select id="books" name="books">
  <option value="fa">Fantasy</option>
  <option value="ho">Horror</option>
  <option value="th">Thriller</option>
  </select>
</form>

</body>
</html>
```
![Alt text](doc-files/sf7.png)

![Alt text](doc-files/sf8.png)

## Responsive Form

```
<!DOCTYPE html>
<html>
<head>
<style>
* {
  box-sizing: border-box;
}

input[type=text], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ffffff;
  border-radius: 4px;
  resize: vertical;
}

label {
  padding: 12px 12px 12px 0;
  display: inline-block;
}

input[type=submit] {
  background-color: #374ef9;
  color: white;
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  float: right;
}

input[type=submit]:hover {
  background-color: #0510a7;
}

.container {
  border-radius: 5px;
  background-color: #96b7f9;
  padding: 20px;
}

.col-25 {
  float: left;
  width: 25%;
  margin-top: 6px;
}

.col-75 {
  float: left;
  width: 75%;
  margin-top: 6px;
}

/* Clear floats after the columns */
.row::after {
  content: "";
  display: table;
  clear: both;
}

/* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .col-25, .col-75, input[type=submit] {
    width: 100%;
    margin-top: 0;
  }
}
</style>
</head>
<body>

<h2>Responsive Form</h2>
<p>Resize the browser window to see columns stack on top of each other instead of next to each other.</p>

<div class="container">
  <form action="/action_page.php">
  <div class="row">
    <div class="col-25">
      <label for="fname">First Name</label>
    </div>
    <div class="col-75">
      <input type="text" id="fname" name="firstname" placeholder="Your name..">
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="lname">Last Name</label>
    </div>
    <div class="col-75">
      <input type="text" id="lname" name="lastname" placeholder="Your last name..">
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="country">Country</label>
    </div>
    <div class="col-75">
      <select id="country" name="country">
        <option value="australia">Australia</option>
        <option value="canada">Canada</option>
        <option value="usa">USA</option>
      </select>
    </div>
  </div>
  <div class="row">
    <div class="col-25">
      <label for="subject">Subject</label>
    </div>
    <div class="col-75">
      <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>
    </div>
  </div>
  <br>
  <div class="row">
    <input type="submit" value="Submit">
  </div>
  </form>
</div>

</body>
</html>
```

![Alt text](doc-files/sf9.png)


