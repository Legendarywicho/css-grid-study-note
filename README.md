# CSS Grid Course
### Css Fundamentals
What is  a grid in CSS
The main idea of grid is slicing a main div into columns and rows. Once you do that you can insert elements into any place of the grid.
### Main properties of Grid
```
<div class="container">
    <div class="item">1</div>
    <div class="item">2</div>
    <div class="item">3</div>
    <div class="item">4</div>
    <div class="item">5</div>
    <div class="item">6</div>
    <div class="item">7</div>
    <div class="item">8</div>
    <div class="item">9</div>
    <div class="item">10</div> 
  </div>
  ````
```
.container{
    display: grid;
    grid-template-columns: 200px auto 50px;
    grid-gap: 20px;
  }
```

#### If you don't implecity define de number of columns it will explicitly define it as one.

### CSS attributes
This makes de container into a grid layout.
```
display: grid;
```
This makes the item inside the grid have a margin or space between the elements
```
grid-gap: 20px;
```
This makes the the first two columns have a width of 400px and 200px , the rest that are implecitly created will be shown into de bottom as a row.
```
grid-template-columns: 400px 200px;
```
This makes the grid elements be placed into a certain pattern which is column or row.
```
grid-auto-flow: column;
```
All of the items that are generated implecitly are going to have a width of 200px 
```
grid-auto-columns: 200px;
```
## Giving a real size to our grid
Fractional Unit - Represents the amount of space left
### example used in CSS
`1 fr`
Usage
`grid-template-columns:  1fr;`

The repeat function can help ous out typing less code to achive the same result

normal way : 
```
grid-template-columns: 1fr 1fr 1fr 1fr;
```
better way : 
```
grid-template-columns: repeat(4,1fr);
```
This is for position more than one spot to an element on the grid layout
```
grid-column: span 10;
grid-row: span 2;
```















