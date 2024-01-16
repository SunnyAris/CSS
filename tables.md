# Borders

```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid;
}
</style>
</head>
<body>

<h2>Add a border to a table:</h2>

<table>
  <tr>
    <th>Genre</th>
    <th>Author</th>
    <th>Title</th>
  </tr>
  <tr>
    <td>Horror</td>
    <td>Stephen King</td>
    <td>The Shining</td>
  </tr>
  <tr>
    <td>Science Fiction </td>
    <td>Frank Herbert</td>
    <td>Dune</td>
  </tr>
  <tr>
    <td>Detective</td>
    <td>Arthur Conan Doyle</td>
    <td>Sherlock Holmes</td>
  </tr>
</table>

</body>
</html>
```
![Alt text](doc-files/tb1.png)

## Full-Width table

```
<!DOCTYPE html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid;
}

table {
  width: 100%;
}
</style>
</head>
<body>

<h2>Full-width Table</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Stephen</td>
    <td>King</td>
  </tr>
  <tr>
    <td>Frank</td>
    <td>Herbert</td>
  </tr>
</table>

</body>
</html>
```

![Alt text](doc-files/tb2.png)

## `border-collapse`

```
<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid;
}

table {
  width: 100%;
  border-collapse: collapse;
}
</style>
</head>
<body>

<h2>Let the table borders collapse</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Stephen</td>
    <td>King</td>
  </tr>
  <tr>
    <td>Frank</td>
    <td>Herbert</td>
  </tr>
</table>

</body>
</html>
```
![Alt text](doc-files/tb3.png)



```
<!DOCTYPE html>
<html>
<head>
<style>
table {
  width: 100%;
  border: 1px solid;
}
</style>
</head>
<body>

<h2>Single Border Around The Table</h2>

<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
  </tr>
  <tr>
    <td>Stephen</td>
    <td>King</td>
  </tr>
  <tr>
    <td>Frank</td>
    <td>Herbert</td>
  </tr>
</table>

</body>
</html>
```
![Alt text](doc-files/tb4.png)

## Width and height

```
<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 100%;
}

th {
  height: 70px;
}
</style>
</head>
<body>

<h2>The width and height properties</h2>

<table>
  <tr>
    <th>Genre</th>
    <th>Author</th>
    <th>Title</th>
  </tr>
  <tr>
    <td>Horror</td>
    <td>Stephen King</td>
    <td>The Shining</td>
  </tr>
  <tr>
    <td>Science Fiction </td>
    <td>Frank Herbert</td>
    <td>Dune</td>
  </tr>
  <tr>
    <td>Detective</td>
    <td>Arthur Conan Doyle</td>
    <td>Sherlock Holmes</td>
  </tr>
</table>

</body>
</html>
```
![Alt text](doc-files/tb5.png)



```
<!DOCTYPE html>
<html>
<head>
<style>
table, td, th {
  border: 1px solid black;
}

table {
  border-collapse: collapse;
  width: 50%;
}
</style>
</head>
<body>

<h2>A table that only span half the page</h2>

<p>Width of the table to 50%:</p>

<table>
  <tr>
    <th>Genre</th>
    <th>Author</th>
    <th>Title</th>
  </tr>
  <tr>
    <td>Horror</td>
    <td>Stephen King</td>
    <td>The Shining</td>
  </tr>
  <tr>
    <td>Science Fiction </td>
    <td>Frank Herbert</td>
    <td>Dune</td>
  </tr>
  <tr>
    <td>Detective</td>
    <td>Arthur Conan Doyle</td>
    <td>Sherlock Holmes</td>
  </tr>
</table>

</body>
</html>
```

![Alt text](doc-files/tb6.png)

