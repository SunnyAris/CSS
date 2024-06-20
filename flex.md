# Flex container

## flex-direction - property defines in which direction the container wants to stack the flex items.

### column value stacks the flex items vertically (from top to bottom):

```
.flex-container {
  display: flex;
  flex-direction: column;
}
```

### column-reverse value stacks the flex items vertically (but from bottom to top):

```
.flex-container {
  display: flex;
  flex-direction: column-reverse;
}
```
### row value stacks the flex items horizontally (from left to right):

```
.flex-container {
  display: flex;
  flex-direction: row;
}
```
### row-reverse value stacks the flex items horizontally (but from right to left):

```
.flex-container {
  display: flex;
  flex-direction: row-reverse;
}
```


## flex-wrap - property specifies whether the flex items should wrap or not.

### wrap value specifies that the flex items will wrap if necessary:

```
.flex-container {
  display: flex;
  flex-wrap: wrap;
}
```

### nowrap value specifies that the flex items will not wrap (this is default):

```
.flex-container {
  display: flex;
  flex-wrap: nowrap;
}
```
### wrap-reverse value specifies that the flexible items will wrap if necessary, in reverse order:

```
.flex-container {
  display: flex;
  flex-wrap: wrap-reverse;
}
```

## flex-flow - flex-flow property is a shorthand property for setting both the flex-direction and flex-wrap properties.

```
.flex-container {
  display: flex;
  flex-flow: row wrap;
}
```

## justify-content - justify-content property is used to align the flex items:

## center value aligns the flex items at the center of the container:

```
.flex-container {
  display: flex;
  justify-content: center;
}
```
![Alt text](doc-files/f12.png)

### flex-end value aligns the flex items at the end of the container:

```
.flex-container {
  display: flex;
  justify-content: flex-end;
}
```

![Alt text](doc-files/f13.png)

### space-around value displays the flex items with space before, between, and after the lines:

```
.flex-container {
  display: flex;
  justify-content: space-around;
}
```
![Alt text](doc-files/f14.png)

### space-between value displays the flex items with space between the lines:

```
.flex-container {
  display: flex;
  justify-content: space-between;
}
```
![Alt text](doc-files/f15.png)

## align-items - align-items property is used to align the flex items.

### center value aligns the flex items in the middle of the container:

```
.flex-container {
  display: flex;
  height: 200px;
  align-items: center;
}
```
### flex-start value aligns the flex items at the top of the container:
```
.flex-container {
  display: flex;
  height: 200px;
  align-items: flex-start;
}
```

### flex-end value aligns the flex items at the bottom of the container:
```
.flex-container {
  display: flex;
  height: 200px;
  align-items: flex-end;
}
```

### stretch value stretches the flex items to fill the container (this is default):

```
.flex-container {
  display: flex;
  height: 200px;
  align-items: stretch;
}
```

### baseline value aligns the flex items such as their baselines aligns:


```
.flex-container {
  display: flex;
  height: 200px;
  align-items: baseline;
}
```
![Alt text](doc-files/f16.png)


## align-content - property is used to align the flex lines.

### space-between value displays the flex lines with equal space between them:

```
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: space-between;
}
```
### space-around value displays the flex lines with space before, between, and after them:

```
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: space-around;
}
```

### stretch value stretches the flex lines to take up the remaining space (this is default):

```
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: stretch;
}
```

### center value displays the flex lines in the middle of the container:

```
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: center;
}
```
### flex-start value displays the flex lines at the start of the container:

```
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: flex-start;
}
```

### flex-end value displays the flex lines at the end of the container: 

```
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: flex-end;
}
```

# Perfect Centering

justify-content and align-items properties to center, and the flex item will be perfectly centered:

```
.flex-container {
  display: flex;
  height: 300px;
  justify-content: center;
  align-items: center;
}
```

## order

```
<div class="flex-container">
  <div style="order: 3">1</div>
  <div style="order: 2">2</div>
  <div style="order: 4">3</div>
  <div style="order: 1">4</div>
</div>
```

##  flex-grow 

the third flex item grow eight times faster
```
<div class="flex-container">
  <div style="flex-grow: 1">1</div>
  <div style="flex-grow: 1">2</div>
  <div style="flex-grow: 8">3</div>
</div>
```

## flex-shrink
how much a flex item will shrink

```
<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div style="flex-shrink: 0">3</div>
  <div>4</div>
  <div>5</div>
  <div>6</div>
  <div>7</div>
  <div>8</div>
  <div>9</div>
  <div>10</div>
</div>
```
## flex-basis

```
<div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div style="flex-basis: 200px">3</div>
  <div>4</div>
</div>
```

## align-self 

Align the second flex item at the top of the container, and the third flex item at the bottom of the container

```
<div class="flex-container">
  <div>1</div>
  <div style="align-self: flex-start">2</div>
  <div style="align-self: flex-end">3</div>
  <div>4</div>
</div>
```


