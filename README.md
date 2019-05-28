# CSS Grid Properties

```css
/* BASICS */
display: grid; /* Specify a grid container */
grid-gap: 1rem; /* Specify the global gutter for rows and columns */
grid-template-columns: 6rem 12rem; /* Define the dimensions of columns */
grid-auto-columns: 2rem; /* Define the dimensions of rows not defined with grid-template-columns */
grid-template-rows: 2rem 4rem; /* Define the dimensions of rows */
grid-auto-rows: 2rem; /* Define the dimesions of rows not defined with grid-template-rows */
grid-auto-flow: column; /* Similar to flex-wrap, determines whether to keep grid items in a single row or wrap them to multiple. Uses the value of grid-auto-columns or grid-auto-rows for dimensions. */

/* TRACK SIZING */
grid-template-columns: 200px 200px 1fr; /* 1 fractional unit will take the remaining space. */
grid-template-columns: auto 1fr; /* First column will fit to content, 2nd will take the remaining space. */

/* REPEAT FUNCTION */
grid-template-columns: 100px repeat(2, 1fr auto) 200px repeat(3, 100px 200px); /* Takes the number of times to repeat a pattern of columns or rows, then a space separated set of dimensions to loop through. */

/* SPANNING ROWS AND COLUMNS */
grid-column: span 8; /* This will create implicit columns beyond 5 columns as defined by the repeat function. */
grid-row: span 2; /* This will make the item 2 rows high, displacing the items that would have flowed there.

```
