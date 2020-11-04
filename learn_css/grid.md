### CSS Grid Essentials
-  grid container and grid items
- `display: grid;`
- `grid-template-columns: 100px 200px;` define the columns of our grid, The first column will be 100 pixels wide and the second column will be 200 pixels wide.
- `grid-template-columns/rows: 20px 40% 60px;`
-  `grid-template: 200px 300px(rows) / 20% 10% 70%;`
- `fr` Fraction
    - `grid-template-columns: 1fr 60px 1fr;`
- Repeat`grid-template-columns: repeat(3, 100px);`
- `minmax(100px, 500px)` always be between 100 and 500 pixels wide in size as the overall grid resizes
----
- `grid-column/row-gap: 10px;` blank space between every row and column in the grid
    - does not add space at the beginning or end of the grid
    - `grid-gap: 20px 10px;` (does not take a `/`)
--- 
#### Multiple Row Items
- `grid-area: 6 / 8 / span 3 / span 1;;`

``` css
/* accept are grid lines */
.item {
  grid-row-start: 1;
  grid-row-end: 3;
  /* or  grid-row/column: 1 / 3; */
}
```
- **span** `grid-column: 4 / span 2;` take up two columns of space

### Advanced CSS Grid
- `grid-template-areas`
``` css
    .container {
        grid-template-areas: "header header"
                              "nav nav"
                              "left right"
                              "footer footer";
    }
    header {
      grid-area: header;
    }

```
- `z-index`: ability to easily overlap elements
--- 
- `justify-items:` positions grid items along the inline, or row, axis
    - `start` / `end`/ `center`/ `stretch`
- `justify-content:`position a grid within its parent element.
    - `start`/ `end`/`center`/ `stretch`
    - `space-around`:includes an equal amount of space on each side of a grid element, resulting in double the amount of space between elements as there is before the first and after the last element
    - `space-between`: includes an equal amount of space between grid items and no space at either end
    - `space-evenly`: places an even amount of space between grid items and at either end
- `align-items:`position grid items from top to bottom
    - `start`/ `end`/`center`/ `stretch`
- `align-content:` positions the rows along the column axis, or from top to bottom
    - `start`/ `end`/`center`/ `stretch`/`space-around`/ `space-between`/ `space-evenly`
- `justify-self:`how an individual element should position itself with respect to the row axis.
    -  This property will override justify-items for any item on which it is declared.
- `align-self:` how an individual element should position itself with respect to the column axis
    - This property will override align-items for any item on which it is declared.
- [Box alignment in CSS Grid Layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Box_Alignment_in_CSS_Grid_Layout#Aligning_the_grid_tracks_on_the_block_or_column_axis)
---
#### Grid Auto Rows and Grid Auto Columns
- `grid-auto-rows` and `grid-auto-columns`
    ``` css
    /* The fifth <div> will be added to an implicit row that will be 50 pixels tall. */
    body {
      display: grid;
      grid: repeat(2, 100px) / repeat(2, 150px); 
      grid-auto-rows: 50px;
    }
    ```
    - `row` — specifies the new elements should fill rows from left to right and create new rows when there are too many elements (default)
    - `column` — specifies the new elements should fill columns from top to bottom and create new columns when there are too many elements
    - `dense` — this keyword invokes an algorithm that attempts to fill holes earlier in the grid layout if smaller elements are added