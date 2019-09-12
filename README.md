# CSS Grid

This project is a sample of how to use the grid system from CSS.

We can separate the grid system in two main groups, called `container` and `item(s)`, which will be
explained above.


## Container

The container is the grid area itself. It delimits the area that represents the grid.
We can see some important container's properties below:

- display: grid;  
  Set the element as a GRID.

- grid-template-columns: 3fr 1fr;  
  Set the amount of columns that the grid will hold and the screen fraction that each column will occupy.
  
  ```
  /* Two columns: The first with 3 fractions of screen and the second with 1 fraction of screen. */
  grid-template-columns: 3fr 1fr;
  ```

- grid-template-rows: 20vh 70vh 10vh;  
  Set the amount of rows that the grid will hold and the screen fraction that each row will occupy.

  ```
  /* Three rows */
  grid-template-rows: 20vh 70vh 10vh;
  ```

- grid-gap: 20px;  
  Set the space between columns and rows.

- grid-template-areas: "header header"
                       "main aside"
                       "footer footer";  
  Inform which item that contains the property `grid-areas` with the same value that should be positioned
  in the specified column and row.

  E.g: "header header" indicates that the item which contains `grid-area: header;`  should be positioned
  in the first and second columns and in the first row.
  

## Item

The item is an element inside a grid. It can be positioned in columns and rows as you need it.
We can see some important items' properties below:

- grid-column-start: 1;  
  Set in which column the item must start.

- grid-column-end: 3;  
  Set in which column the item must end.

- grid-column: 1/3;  
  It's a shortcut for `grid-column-start` and `grid-column-end` above.

- grid-areas: header;  
  Set the grid area name.


## Positioning

There are 6 positioning properties:

-  `justify-content`
-  `align-content`
-  `justify-items`
-  `align-items`
-  `justify-self`
-  `align-self`

### Content

-  `justify-content` (X axis) and `align-content` (Y axis) allow us to position the grid itself, relative to the space around it. These properties can have the following values:

1. start
2. end
3. center
4. stretch
5. space-between
6. space-around
7. space-evenly

### Items

-  `justify-items` and `align-items` allow us to position all the grid's items, relative to the available space the inside cell where the item is in. These properties can have the following values:

1. start
2. end
3. center
4. stretch

### Self

-  `justify-self` and `align-self` allow us to position a specific item, relative to the available space inside the cell where the item is in. These properties can have the following values:

1. start
2. end
3. center
4. stretch
