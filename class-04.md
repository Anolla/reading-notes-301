# Responsive Web Design and Regular Expressions

- CSS Grid Layout (aka "Grid"), is a two-dimensional grid-based layout system that aims to do nothing less than completely change the way we design grid-based user interfaces.

### Properties for the Parent
(Grid Container)

display
Defines the element as a grid container and establishes a new grid formatting context for its contents.

Values:

grid - generates a block-level grid
inline-grid - generates an inline-level grid
container {
  display: grid | inline-grid;
}


### Properties for the Children
(Grid Items)

grid-column-start
grid-column-end
grid-row-start
grid-row-end
Determines a grid item's location within the grid by referring to specific grid lines. grid-column-start/grid-row-start is the line where the item begins, and grid-column-end/grid-row-end is the line where the item ends.

Values:

<line> - can be a number to refer to a numbered grid line, or a name to refer to a named grid line
span <number> - the item will span across the provided number of grid tracks
span <name> - the item will span across until it hits the next line with the provided name
auto - indicates auto-placement, an automatic span, or a default span of one
item {
  grid-column-start: <number> | <name> | span <number> | span <name> | auto;
  grid-column-end: <number> | <name> | span <number> | span <name> | auto;
  grid-row-start: <number> | <name> | span <number> | span <name> | auto;
  grid-row-end: <number> | <name> | span <number> | span <name> | auto;
}


### grid-template-areas
Defines a grid template by referencing the names of the grid areas which are specified with the grid-area property. Repeating the name of a grid area causes the content to span those cells. A period signifies an empty cell. The syntax itself provides a visualization of the structure of the grid.

Values:

<grid-area-name> - the name of a grid area specified with grid-area
- a period signifies an empty grid cell
none - no grid areas are defined
container {
  grid-template-areas: 
    "<grid-area-name> | . | none | ..."
    "...";
}

### grid-column-gap
grid-row-gap
Specifies the size of the grid lines. You can think of it like setting the width of the gutters between the columns/rows.

Values:

<line-size> - a length value
container {
  grid-column-gap: <line-size>;
  grid-row-gap: <line-size>;
}

### align-items
Aligns grid items along the block (column) axis (as opposed to justify-items which aligns along the inline (row) axis). This value applies to all grid items inside the container.

Values:

start - aligns items to be flush with the start edge of their cell
end - aligns items to be flush with the end edge of their cell
center - aligns items in the center of their cell
stretch - fills the whole height of the cell (this is the default)
container {
  align-items: start | end | center | stretch;
}
Examples:

.container {
  align-items: start;
}

### align-content
Sometimes the total size of your grid might be less than the size of its grid container. This could happen if all of your grid items are sized with non-flexible units like px. In this case you can set the alignment of the grid within the grid container. This property aligns the grid along the block (column) axis (as opposed to justify-content which aligns the grid along the inline (row) axis).

Values:

start - aligns the grid to be flush with the start edge of the grid container
end - aligns the grid to be flush with the end edge of the grid container
center - aligns the grid in the center of the grid container
stretch - resizes the grid items to allow the grid to fill the full height of the grid container
space-around - places an even amount of space between each grid item, with half-sized spaces on the far ends
space-between - places an even amount of space between each grid item, with no space at the far ends
space-evenly - places an even amount of space between each grid item, including the far ends
container {
  align-content: start | end | center | stretch | space-around | space-between | space-evenly;	
}

