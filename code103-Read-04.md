# Responsive Web Design and Regular Expressions

![grid](https://miro.medium.com/max/2800/0*MJfiLHUiFLi5M2sm.png)

### display
Defines the element as a grid container and establishes a new grid formatting context for its contents.

**Values:**
* grid – generates a block-level grid
* inline-grid – generates an inline-level grid

**Note:**
float, display: inline-block, display: table-cell, vertical-align and column-* properties have no effect on a grid item.
[grid2](https://miro.medium.com/max/2482/1*IOo53ZeAYqhE6CwHQhOOZw.gif)

### grid-template-columns and grid-template-rows
Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.

### grid-column-start, grid-column-end, grid-row-start, grid-row-end
Determines a grid item’s location within the grid by referring to specific grid lines. grid-column-start/grid-row-start is the line where the item begins, and grid-column-end/grid-row-end is the line where the item ends.

### grid-area
Gives an item a name so that it can be referenced by a template created with the grid-template-areas property.

### grid-template-areas
Defines a grid template by referencing the names of the grid areas which are specified with the grid-area property. 

### justify-self
Aligns a grid item inside a cell along the inline (row) axis (as opposed to align-self which aligns along the block (column) axis).
![justify](https://discourse.wicg.io/uploads/default/original/1X/37139f17fecbf735cd165ba8c7e5d6e98db13667.jpg)

### align-self
Aligns a grid item inside a cell along the block (column) axis (as opposed to justify-self which aligns along the inline (row) axis).

![align](https://devopedia.org/images/article/179/3246.1559055714.png)

### column-gap, row-gap, grid-column-gap, grid-row-gap
Specifies the size of the grid lines. You can think of it like setting the width of the gutters between the columns/rows.

### justify-items
Aligns grid items along the inline (row) axis (as opposed to align-items which aligns along the block (column) axis). 

### align-items
Aligns grid items along the block (column) axis (as opposed to justify-items which aligns along the inline (row) axis). 

### place-items
place-items sets both the align-items and justify-items properties in a single declaration.

### align-content
Sometimes the total size of your grid might be less than the size of its grid container. 