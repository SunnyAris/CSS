## Rounded Corners

```
<!DOCTYPE html>
<html>
<head>
<style> 
#rcorners1 {
  border-radius: 25px;
  background: #90bff8;
  padding: 20px; 
  width: 200px;
  height: 150px;  
}

#rcorners2 {
  border-radius: 25px;
  border: 2px solid #73AD21;
  padding: 20px; 
  width: 200px;
  height: 150px;  
}

#rcorners3 {
  border-radius: 25px;
  background: url(doc-files/cloudb.jpg);
  background-position: left top;
  background-repeat: repeat;
  padding: 20px; 
  width: 200px;
  height: 150px;  
}
</style>
</head>
<body>

<h1>The border-radius Property</h1>

<p>Rounded corners for an element with a specified background color:</p>
<p id="rcorners1">Rounded corners</p>
<p>Rounded corners for an element with a border:</p>
<p id="rcorners2">Rounded corners</p>
<p>Rounded corners for an element with a background image:</p>
<p id="rcorners3">Rounded corners</p>

</body>
</html>
```
![Alt text](doc-files/rc.png)

```
<!DOCTYPE html>
<html>
<head>
<style> 
#rcorners1 {
  border-radius: 15px 50px 30px 5px;
  background: cornflowerblue;
  padding: 20px; 
  width: 100px;
  height: 100px; 
}

#rcorners2 {
  border-radius: 15px 50px 30px;
  background: cornflowerblue;
  padding: 20px; 
  width: 100px;
  height: 100px; 
}

#rcorners3 {
  border-radius: 15px 50px;
  background: cornflowerblue;
  padding: 20px; 
  width: 100px;
  height: 100px; 
} 

#rcorners4 {
  border-radius: 15px;
  background: cornflowerblue;
  padding: 20px; 
  width: 100px;
  height: 100px; 
} 
</style>
</head>
<body>

<p>Four values - border-radius: 15px 50px 30px 5px:</p>
<p id="rcorners1"></p>

<p>Three values - border-radius: 15px 50px 30px:</p>
<p id="rcorners2"></p>

<p>Two values - border-radius: 15px 50px:</p>
<p id="rcorners3"></p>

<p>One value - border-radius: 15px:</p>
<p id="rcorners4"></p>

</body>
</html>
```
![Alt text](doc-files/rc1.png)

```
<!DOCTYPE html>
<html>
<head>
<style> 
#rcorners1 {
  border-radius: 50px / 15px;
  background: cornflowerblue;
  padding: 20px; 
  width: 100px;
  height: 100px; 
}

#rcorners2 {
  border-radius: 15px / 50px;
  background: cornflowerblue;
  padding: 20px; 
  width: 100px;
  height: 100px; 
}

#rcorners3 {
  border-radius: 50%;
  background: cornflowerblue;
  padding: 20px; 
  width: 100px;
  height: 100px;
} 
</style>
</head>
<body>

<p>Elliptical border - border-radius: 50px / 15px:</p>
<p id="rcorners1"></p>

<p>Elliptical border - border-radius: 15px / 50px:</p>
<p id="rcorners2"></p>

<p>Ellipse border - border-radius: 50%:</p>
<p id="rcorners3"></p>

</body>
</html>
```
![Alt text](doc-files/rc2.png)


