



Grid
Create a fully responsive, fluid and nestable grid layout.

The Grid system of UIkit allows you to arrange block elements in columns. It works closely together with the Width component to determine how much space of the container each item will take up, and it can also be combined with the Flex component to align and order grid items.

Usage
To create the grid container, add the uk-grid attribute to a <div> element. Add child <div> elements to create the cells. By default, all grid cells are stacked. To place them side by side, add one of the classes from the Width component. Using .uk-child-width-expand will automatically apply equal width to items, regardless of how many there are.

NOTE There's no need to add a .uk-grid class as it will be added via JavaScript. However, if UIkit's JavaScript is deferred, the class should be added to prevent stacking while loading.

<div uk-grid>
    <div></div>
    <div></div>
</div>
NOTE Often cards from the Card component are used inside a grid. This also goes for the following examples for visualization.

PREVIEW
MARKUP
Item
Item
Item


<div class="uk-child-width-expand@s uk-text-center" uk-grid>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
</div>



Gutter modifiers
The Grid component comes with a default gutter that is decreased automatically from a certain breakpoint usually on a smaller desktop viewport width. To apply a different gutter, add one of the following classes.

CLASS	DESCRIPTION
.uk-grid-small	Add this class to apply a small gutter.
.uk-grid-medium	Add this class to apply a medium gutter like the default one, but without a breakpoint.
.uk-grid-large	Add this class to apply a large gutter with breakpoints.
.uk-grid-collapse	Add this class to remove the grid gutter entirely.
<div class="uk-grid-small" uk-grid>...</div>
PREVIEW
MARKUP
Item
Item
Item
PREVIEW
MARKUP
Item
Item
Item
PREVIEW
MARKUP
Item
Item
Item
PREVIEW
MARKUP
Item
Item
Item


<div class="uk-grid-collapse uk-child-width-expand@s uk-text-center" uk-grid>
    <div>
        <div class="uk-background-muted uk-padding">Item</div>
    </div>
    <div>
        <div class="uk-background-primary uk-padding uk-light">Item</div>
    </div>
    <div>
        <div class="uk-background-secondary uk-padding uk-light">Item</div>
    </div>
</div>


Nested grid
You can easily extend your grid layout with nested grids.

<div uk-grid>
    <div>
        <div uk-grid>
            <div></div>
            <div></div>
        </div>
    </div>
    <div>
        <div uk-grid>
            <div></div>
            <div></div>
        </div>
    </div>
</div>
PREVIEW
MARKUP
Item
Item
Item


<div class="uk-child-width-1-2 uk-text-center" uk-grid>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-child-width-1-2 uk-text-center" uk-grid>
            <div>
                <div class="uk-card uk-card-primary uk-card-body">Item</div>
            </div>
            <div>
                <div class="uk-card uk-card-primary uk-card-body">Item</div>
            </div>
        </div>
    </div>
</div>



Divider modifier
Add the .uk-grid-divider class to separate grid cells with lines. This class can be combined with the gutter modifiers. As soon as the grid stacks, the divider lines will become horizontal.

<div class="uk-grid-divider" uk-grid>...</div>
PREVIEW
MARKUP
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
Match height
To match the height of the direct child of each cell, add the .uk-grid-match class. This is needed to match the height of cards from the Card component.

<div class="uk-grid-match" uk-grid>....</div>
PREVIEW
MARKUP
Item
Item
...
Item
...
...


<div class="uk-grid-divider uk-child-width-expand@s" uk-grid>
    <div>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</div>
    <div>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
    <div>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</div>
</div>



Match only one cell
You can also match the height of the direct child of just one cell. To do so, add the .uk-grid-item-match class to the grid item whose child you want to match.

<div uk-grid>
    <div class="uk-grid-item-match"></div>
    <div></div>
</div>
PREVIEW
MARKUP
Heading
Lorem ipsum dolor sit amet.

Heading
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

JavaScript
For a more specific selection of the elements whose heights should be matched, add the target: SELECTOR option to the uk-height-match attribute from the Height component.

<div uk-grid uk-height-match="target: > div > .uk-card">
    <div>
        <div class="uk-card uk-card-default"></div>
    </div>
    <div>
        <div class="uk-card uk-card-default"></div>
    </div>
</div>
PREVIEW
MARKUP
Item
Item
...
Item
...
...


<div class="uk-child-width-expand@s" uk-grid>
    <div class="uk-grid-item-match">
        <div class="uk-card uk-card-default uk-card-body">
            <h3>Heading</h3>
            <p>
                Lorem ipsum dolor sit amet.
            </p>
        </div>
     </div>
    <div>
        <h3>Heading</h3>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        </p>
    </div>
</div>



<div class="uk-child-width-expand@s uk-text-center" uk-grid uk-height-match="target: > div > .uk-card">
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
     </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item<br>...</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item<br>...<br>...</div>
    </div>
</div>



Grid and width
The grid is mostly used in combination with the Width component. This allows for great flexibility when determining the column widths.

<div uk-grid>
    <div class="uk-width-auto@m"></div>
    <div class="uk-width-1-3@m"></div>
    <div class="uk-width-expand@m"></div>
</div>
PREVIEW
MARKUP
Auto
1-3
Expand


<div class="uk-text-center" uk-grid>
    <div class="uk-width-auto@m">
        <div class="uk-card uk-card-default uk-card-body">Auto</div>
    </div>
    <div class="uk-width-1-3@m">
        <div class="uk-card uk-card-default uk-card-body">1-3</div>
    </div>
    <div class="uk-width-expand@m">
        <div class="uk-card uk-card-default uk-card-body">Expand</div>
    </div>
</div>



Child width
If the grid columns are evenly split, you can add one of the .uk-child-width-* classes to the grid container instead of adding a class to each of the items.

<div class="uk-child-width-1-2@s uk-child-width-1-3@m" uk-grid>...</div>
PREVIEW
MARKUP
Item
Item
Item
For more detailed information, take a look at the Width component.


<div class="uk-child-width-1-2@s uk-child-width-1-3@m uk-text-center" uk-grid>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
</div>


Grid and flex
You can easily combine the grid with the Flex component. That way you can modify the items' alignment, ordering, direction and wrapping. This allows you, for example, to flip the cells' display order for wider viewports. All this works together with the gutter and divider modifiers.

<div class="uk-flex-center" uk-grid>
    <div></div>
    <div class="uk-flex-first"></div>
</div>
PREVIEW
MARKUP
Item 1
Item 2
Item 3
Item 4
Item 5
Item 6

<div class="uk-grid-small uk-child-width-1-4@s uk-flex-center uk-text-center" uk-grid>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item 1</div>
    </div>
    <div class="uk-flex-last">
        <div class="uk-card uk-card-secondary uk-card-body">Item 2</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item 3</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item 4</div>
    </div>
    <div class="uk-flex-first">
        <div class="uk-card uk-card-primary uk-card-body">Item 5</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item 6</div>
    </div>
</div>



Masonry
If grid cells have different heights, a layout free of gaps can be created by adding masonry: true to the attribute.

<div uk-grid="masonry: true">...</div>
PREVIEW
MARKUP
Item
Item
Item
Item
Item
Item
Item
Item
Item


<div class="uk-child-width-1-2@s uk-child-width-1-3@m" uk-grid="masonry: true">
    <div>
        <div class="uk-card uk-card-default uk-flex uk-flex-center uk-flex-middle" style="height: 100px">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-flex uk-flex-center uk-flex-middle" style="height: 130px">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-flex uk-flex-center uk-flex-middle" style="height: 150px">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-flex uk-flex-center uk-flex-middle" style="height: 160px">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-flex uk-flex-center uk-flex-middle" style="height: 120px">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-flex uk-flex-center uk-flex-middle" style="height: 140px">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-flex uk-flex-center uk-flex-middle" style="height: 200px">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-flex uk-flex-center uk-flex-middle" style="height: 180px">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-flex uk-flex-center uk-flex-middle" style="height: 140px">Item</div>
    </div>
</div>




NOTE You can view more examples in the tests for the Grid Masonry.

Filter and order
Grid items can also be filtered and sorted by category, date or other meta data. Take a look at the Filter component.

Parallax
To move single columns of a grid at different speeds while scrolling, just add parallax: NUMBER to the attribute. The number sets the parallax translation in pixels.

<div uk-grid="parallax: 150">...</div>
This effect can be applied to two types of markup. The following example uses three defined columns with three items each.

PREVIEW
MARKUP
Item
Item
Item
Item
Item
Item
Item
Item
Item

<div class="uk-child-width-expand@s uk-text-center" uk-grid="parallax: 150">
    <div>
        <div class="uk-card uk-card-default uk-card-body uk-grid-margin">Item</div>
        <div class="uk-card uk-card-default uk-card-body uk-grid-margin">Item</div>
        <div class="uk-card uk-card-default uk-card-body uk-grid-margin">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body uk-grid-margin">Item</div>
        <div class="uk-card uk-card-default uk-card-body uk-grid-margin">Item</div>
        <div class="uk-card uk-card-default uk-card-body uk-grid-margin">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body uk-grid-margin">Item</div>
        <div class="uk-card uk-card-default uk-card-body uk-grid-margin">Item</div>
        <div class="uk-card uk-card-default uk-card-body uk-grid-margin">Item</div>
    </div>
</div>



The parallax effect is also applied if grid columns wrap into the next row, as shown in the next example.

PREVIEW
MARKUP
Item
Item
Item
Item
Item
Item
Item
Item
Item
Item
Item
Item



<div class="uk-child-width-1-2@s uk-child-width-1-3@m uk-child-width-1-4@l uk-text-center" uk-grid="parallax: 150">
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">Item</div>
    </div>
</div>



NOTE You can view more examples in the Grid Parallax tests.

Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
margin	String	uk-grid-margin	This class is added to items that break into the next row, typically to create margin to the previous row.
first-column	String	uk-first-column	This class is added to the first element in each row.
masonry	Boolean	false	Enables masonry layout for this grid.
parallax	Number	0	Parallax translation value. The value must be a positive integer. Falsy disables the parallax effect (default).
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.grid(element, options);

