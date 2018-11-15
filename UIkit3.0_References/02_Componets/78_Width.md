


Width
Define the width of elements for different viewport sizes.

UIkit's Width component is often used in combination with grids to split content into responsive columns. You can apply fractions, automatic width or expand units to fill the remaining space and combine these modes.

Usage
Add one of the .uk-width-* classes to an element to determine its size. Typically, you would use a grid from the Grid component and its child elements to create the units.

CLASS	DESCRIPTION
.uk-width-1-1	Fills 100% of the available width.
.uk-width-1-2	The element takes up halves of its parent container.
.uk-width-1-3 to .uk-width-2-3	The element takes up thirds of its parent container.
.uk-width-1-4 to .uk-width-3-4	The element takes up fourths of its parent container.
.uk-width-1-5 to .uk-width-4-5	The element takes up fifths of its parent container.
.uk-width-1-6 to .uk-width-5-6	The element takes up sixths of its parent container.
NOTE We remove redundancy into each set of unit classes, so that for instance instead of .uk-width-3-6 you should use .uk-width-1-2.

<div uk-grid>
    <div class="uk-width-1-2"></div>
    <div class="uk-width-1-2"></div>
</div>
PREVIEW
MARKUP
1-3
1-3
1-3
1-2
1-2
1-4
3-4
Auto & expand
The Width component provides additional modifiers to give you more flexibility in the distribution of items.

CLASS	DESCRIPTION
.uk-width-auto	The item expands only to the width of its own content.
.uk-width-expand	The item expands to fill up the remaining space of the grid container.
<div uk-grid>
    <div class="uk-width-auto"></div>
    <div class="uk-width-expand"></div>
</div>
PREVIEW
MARKUP
Auto
Expand
Equal child widths
To create a grid whose child elements' widths are evenly split, you don't have to apply the same class to each list item within the grid. Just add one of the .uk-child-width-* classes to the grid itself.

CLASS	DESCRIPTION
.uk-child-width-1-2	All elements take up half of their parent container.
.uk-child-width-1-3	All elements take up a third of their parent container.
.uk-child-width-1-4	All elements take up a fourth of their parent container.
.uk-child-width-1-5	All elements take up a fifth of their parent container.
.uk-child-width-1-6	All elements take up a sixth of their parent container.
.uk-child-width-auto	Divides the grid into equal units depending on the content size.
.uk-child-width-expand	Divides the grid into equal units depending on the available space.
<div class="uk-child-width-1-4" uk-grid>
    <div></div>
    <div></div>
    ...
</div>
PREVIEW
MARKUP
Item
Item
Item
Item
Item
Items that use width classes with fractions will break into a new row, if they no longer fit their container's width. When using one of the expand classes, however, the space will be evenly distributed among items that always stay in the same row.

<div class="uk-child-width-expand" uk-grid>
    <div></div>
    <div></div>
    ...
</div>
PREVIEW
MARKUP
Item
Item
Item
Item
Item
Fixed width
In addition to the calculated width classes, you can also add one of the following classes, which apply fixed widths.

CLASS	DESCRIPTION
.uk-width-small	Applies a fixed width of 150px.
.uk-width-medium	Applies a fixed width of 300px.
.uk-width-large	Applies a fixed width of 450px.
.uk-width-xlarge	Applies a fixed width of 600px.
.uk-width-xxlarge	Applies a fixed width of 750px.
<div class="uk-width-medium"></div>
PREVIEW
MARKUP
Small
Medium
Large
X Large
XX Large
Mixing widths
You can also combine .uk-child-width-* classes with .uk-width-* classes for individual items. That way it is possible, for example, to create a grid with one item that has a specific width and all other items expanding to fill the remaining space.

<div class="uk-child-width-expand" uk-grid>
    <div></div>
    <div class="uk-width-1-3"></div>
    <div></div>
    ...
</div>
PREVIEW
MARKUP
Expand
1-3
Expand
Expand
Responsive width
UIkit provides a number of responsive widths classes. Basically they work just like the usual width classes, except that they have suffixes that represent the breakpoint from which they come to effect. These classes can be combined with the Visibility component. This is great to adjust your layout and content for different device sizes.

CLASS	DESCRIPTION
.uk-width-*
.uk-child-width-*	Affects all device widths, grid columns stay side by side.
.uk-width-*@s
.uk-child-width-*@s	Affects device widths of 640px and larger. Grid columns will stack on smaller sizes.
.uk-width-*@m
.uk-child-width-*@m	Affects device widths of 960px and larger. Grid columns will stack on smaller sizes.
.uk-width-*@l
.uk-child-width-*@l	Affects device widths of 1200px and larger. Grid columns will stack on smaller sizes.
.uk-width-*@xl
.uk-child-width-*@xl	Affects device widths of 1600px and larger. Grid columns will stack on smaller sizes.
PREVIEW
MARKUP
1-2@m
1-4@m
1-4@m
1-5@m
1-3@l
3-5@m
2-3@l
auto@m
visible@l
1-3@m
expand@m
