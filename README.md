Creating a fluid grid

Our grid works nicely, but it has a fixed width. We really want a flexible (fluid) grid that will grow and shrink with the available space in the browser viewport. To achieve this we can turn the reference pixel widths into percentages.

The equation that turns a fixed width into a flexible percentage-based one is as follows.

target / context = result

For our column width, our target width is 60 pixels and our context is the 960 pixel wrapper. We can use the following to calculate a percentage.

60 / 960 = 0.0625

We then move the decimal point 2 places giving us a percentage of 6.25%. So, in our CSS we can replace the 60 pixel column width with 6.25%.

We need to do the same with our gutter width:

20 / 960 = 0.02083333333

So we need to replace the 20 pixel margin-left on our .col rule and the 20 pixel padding-right on .wrapper with 2.08333333%.

Updating our grid

To get started in this section, make a new copy of your previous example page.

Ref: https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Legacy_Layout_Methods

Live web: https://gitthuma.github.io/legacy-layout-fluid-grid/
