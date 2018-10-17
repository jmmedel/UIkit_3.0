



Flex
Utilize the power of flexbox to create a wide range of layouts.

The Flex component has an essential role in building layouts in UIkit. A lot of components, for example the Grid as well as horizontal navigations, like the Navbar, Subnav, Breadcrumb, Pagination, Tab and Dotnav are built with flexbox and can be used together with the utility classes from this component.

Usage
To apply the flexbox layout model, use one of the following classes. By default, all flex items are aligned to the left, as wide as their content and matched in height.

CLASS	DESCRIPTION
.uk-flex	Create the flex container and behave like a block element.
.uk-flex-inline	Create the flex container and behave like an inline element.
<div class="uk-flex">
    <div></div>
</div>
PREVIEW
MARKUP
Item 1
Item 2
Item 3
Horizontal alignment
These classes define the horizontal alignment of flex items and distribute the space between them. Add one or more of them to the flex container in order to configure the alignments of the flex items. By default, flex items are aligned to the left as does the .uk-flex-left class.

CLASS	DESCRIPTION
.uk-flex-left	Add this class to align flex items to the left.
.uk-flex-center	Add this class to center flex items along the main axis.
.uk-flex-right	Add this class to align flex items to the right.
.uk-flex-between	Add this class to distribute items evenly, with equal space between the items along the main axis.
.uk-flex-around	Add this class to distribute items evenly with equal space on both sides of each item.
<div class="uk-flex uk-flex-center">
    <div></div>
</div>
PREVIEW
MARKUP
Item 1
Item 2
Item 3
Responsive
UIkit provides a number of responsive flex classes for horizontal alignment. Basically, they work just like the usual flex alignment classes, except that they have suffixes that represent the breakpoint from which they come to effect.

CLASS	DESCRIPTION
.uk-flex-left@s
.uk-flex-center@s
.uk-flex-right@s
.uk-flex-between@s
.uk-flex-around@s	Only affects device widths of 640px and higher.
.uk-flex-left@m
.uk-flex-center@m
.uk-flex-right@m
.uk-flex-between@m
.uk-flex-around@m	Only affects device widths of 960px and higher.
.uk-flex-left@l
.uk-flex-center@l
.uk-flex-right@l
.uk-flex-between@l
.uk-flex-around@l	Only affects device widths of 1200px and higher.
.uk-flex-left@xl
.uk-flex-center@xl
.uk-flex-right@xl
.uk-flex-between@xl
.uk-flex-around@xl	Only affects device widths of 1600px and higher.
<div class="uk-flex uk-flex-center@m uk-flex-right@l">
    <div></div>
</div>
PREVIEW
MARKUP
Item 1
Item 2
Item 3
Vertical alignment
These classes define the vertical alignment of flex items. By default, flex items fill the height of their container as does the .uk-flex-stretch class.

CLASS	DESCRIPTION
.uk-flex-stretch	Add this class to expand flex items to fill the height of their parent.
.uk-flex-top	Add this class to align flex items to the top.
.uk-flex-middle	Add this class to center flex items along the cross axis.
.uk-flex-bottom	Add this class to align flex items to the bottom.
<div class="uk-flex uk-flex-middle"></div>
PREVIEW
MARKUP
Item 1
Item 2
...
Item 3
...
...
Direction modifiers
These classes define the axis that flex items are placed on and their direction. By default, items run horizontally from left to right as does the .uk-flex-row class.

CLASS	DESCRIPTION
.uk-flex-row	Add this class to lay out flex items as horizontal rows.
.uk-flex-row-reverse	Add this class to lay out flex items from right to left.
.uk-flex-column	Add this class to lay out flex items as vertical columns.
.uk-flex-column-reverse	Add this class to lay out flex items from bottom to top.
<div class="uk-flex uk-flex-column"></div>
PREVIEW
MARKUP
Item 1
Item 2
Item 3
Wrap modifiers
By default, flex items are fit into one line and run from left to right. Add one of these classes to modify the behavior of wrapping flex items.

CLASS	DESCRIPTION
.uk-flex-wrap	Add this class to make flex items wrap into another line when they no longer fit their container.
.uk-flex-wrap-reverse	Add this class to change the items' direction so that they run from right to left.
.uk-flex-nowrap	Add this class to force the flex items into one line. This is the default behavior.
The following classes modify the alignment of wrapping flex items.

CLASS	DESCRIPTION
.uk-flex-wrap-stretch	Add this class, so that item lines stretch to take up the remaining space
.uk-flex-wrap-between	Add this class to distribute item lines evenly, with the first row at the top and last row at the bottom of the container.
.uk-flex-wrap-around	Add this class to distribute lines evenly with equal space at the top and bottom of each row.
.uk-flex-wrap-top	Add this class to align multiline flex items to the top.
.uk-flex-wrap-middle	Add this class to vertically center multirow flex items.
.uk-flex-wrap-bottom	Add this class to align multiline flex items to the bottom.
<div class="uk-flex uk-flex-wrap uk-flex-wrap-around"></div>
PREVIEW
MARKUP
Item 1
Item 2
Item 3
Item 4
Item 5
Item 6
Item order
By default, flex items are laid out according to the source order. To display a certain item as the first or last one, just add one of these classes.

CLASS	DESCRIPTION
.uk-flex-first	Displays the item as the first one.
.uk-flex-last	Displays the item as the last one.
.uk-flex-first@s
.uk-flex-last@s	Affects device widths of 640px and higher.
.uk-flex-first@m
.uk-flex-last@m	Affects device widths of 960px and higher.
.uk-flex-first@l
.uk-flex-last@l	Affects device widths of 1200px and higher.
.uk-flex-first@xl
.uk-flex-last@xl	Affects device widths of 1600px and higher.
<div class="uk-flex">
  <div></div>
  <div class="uk-flex-first"></div>
</div>
PREVIEW
MARKUP
Item 1
Item 2
Item 3
Item dimensions
To determine how much space a flex item should take up, add one of the following classes to the item. By default, items determine their size by their content, but are allowed to shrink.

CLASS	DESCRIPTION
.uk-flex-none	The box's size is determined by its content.
.uk-flex-auto	The space is allocated considering the item's content.
.uk-flex-1	The space is allocated solely based on flex.
Flex and grid
The Flex component can be combined with a grid from the Grid component.

PREVIEW
MARKUP
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna.

Image






