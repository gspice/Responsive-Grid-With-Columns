# Responsive Grid With Columns
A responsive grid system that uses Flexbox, Modernizr, and includes fallback styling. Also supports column classes.

Tested back to IE9.

## Requirements
The Responsive Grid uses <a href="https://modernizr.com/">Modernizr</a> to do a Flexbox support check to allow support on newer browsers.

The JS is included in the source files, but if you want to extend the support, head over to their <a href="https://modernizr.com/download?setclasses">Download Page</a> to customize the package.

## Installment
1. Include the `modernizr-flexbox.min.js` file to your document head.
2. Add `responsive-grid.css` to your document head, or include it in your main stylsheet.
3. Build your markup as shown in the `responsive-grid-example.html` file.

## Usage
To use the Responsive Grid, determine how many columns you want in each row. In this example, we want the Grid to be 4 columns wide:

1. Create a wrapper `div` for each row of your grid with a class of `.grid`.
2. Add the desired column class to each row `div`. In this case, `grid-one-fourth` on `.grid`.
3. Add the corresponding number of columns as child elements with the following class: `.grid-box` (in this example, you will add 4 of these).
4. Within each `.grid-box`, add an empty `div` with a class of `.grid-box-content`.
5. To have your content line up correctly along the horizontal axis, you'll need to group content together in `.grid-box-item` classes. See the `responsive-grid-example.html` for an example.
6. If you want an element to stick to the bottom of column (i.e. a CTA), add a `.bottom` class to the `.grid-box-item` class.
7. If you want to stack rows, they should be done with the wrapper `.grid` class for each row. They will stack seemlessly.

## Columns
The Responsive Grid uses default column classes found in the <a href="http://genesistheme.com">Genesis Sample Theme</a> from <a href="http://www.studiopress.com">StudioPress</a>, but with the `.grid-` prefix, to control the layout of the Grid.

## Fallback Support
The Repsonsive Grid uses `table` styling to achieve a controlled height of the grid columns. The only difference is that if buttons are included they will not end up at the bottom of the box. i.e. The `.grid-box-item.bottom` class is unsupported on browsers older than IE 9.
