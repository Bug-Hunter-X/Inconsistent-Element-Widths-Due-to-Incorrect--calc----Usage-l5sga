# Inconsistent Element Widths Due to Incorrect `calc()` Usage

This repository demonstrates a common CSS bug related to the incorrect use of the `calc()` function.  The bug arises from attempting to calculate a width based on a percentage of a parent element's width when that parent element's width itself is not explicitly defined or is dependent on its content.

The `bug.css` file contains the erroneous CSS, and `solution.css` shows the corrected code.

## Bug:
Inconsistent or unexpected element widths, especially across different screen sizes or when parent element's width changes dynamically.

## Solution:
Ensure the parent element has a defined width (e.g., using `width: 500px;` or `width: 100%;`)  before using `calc()` to determine child element widths.  Alternatively, consider using alternative layout techniques such as flexbox or grid to manage element widths more robustly.