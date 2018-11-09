
Sortable
Create sortable grids and lists to rearrange the order of its elements.

Drag and drop an element to a new location within the sortable grid, while the other items adjust to fit. This is great, if you want to sort items like gallery or menu items, for example.

Usage
To apply this component, add the uk-sortable attribute to a container and create child elements.

<div uk-sortable>
    <div></div>
    <div></div>
</div>
PREVIEW
MARKUP
Item 1
Item 2
Item 3
Item 4
Item 5
Item 6
Item 7
Item 8


<ul class="uk-grid-small uk-child-width-1-2 uk-child-width-1-4@s uk-text-center" uk-sortable="handle: .uk-card" uk-grid>
    <li>
        <div class="uk-card uk-card-default uk-card-body">Item 1</div>
    </li>
    <li>
        <div class="uk-card uk-card-default uk-card-body">Item 2</div>
    </li>
    <li>
        <div class="uk-card uk-card-default uk-card-body">Item 3</div>
    </li>
    <li>
        <div class="uk-card uk-card-default uk-card-body">Item 4</div>
    </li>
    <li>
        <div class="uk-card uk-card-default uk-card-body">Item 5</div>
    </li>
    <li>
        <div class="uk-card uk-card-default uk-card-body">Item 6</div>
    </li>
    <li>
        <div class="uk-card uk-card-default uk-card-body">Item 7</div>
    </li>
    <li>
        <div class="uk-card uk-card-default uk-card-body">Item 8</div>
    </li>
</ul>


Handle
By default, the entire sortable element can be used for drag and drop sorting. To create a handle which will be used instead, just add the handle: SELECTOR option to the attribute and add the handle class to the element that you want to use as a handle.

<ul uk-sortable="handle: .uk-sortable-handle">
    <li>
        <div class="uk-sortable-handle"></div>
        ...
    </li>
</ul>
PREVIEW
MARKUP
Item 1
Item 2
Item 3
Item 4
Item 5
Item 6
Item 7
Item 8
Group


<div class="uk-child-width-1-3@s" uk-grid>
    <div>
        <h4>Group 1</h4>
        <div uk-sortable="group: sortable-group">
            <div class="uk-margin">
                <div class="uk-card uk-card-default uk-card-body uk-card-small">Item 1</div>
            </div>
            <div class="uk-margin">
                <div class="uk-card uk-card-default uk-card-body uk-card-small">Item 2</div>
            </div>
            <div class="uk-margin">
                <div class="uk-card uk-card-default uk-card-body uk-card-small">Item 3</div>
            </div>
            <div class="uk-margin">
                <div class="uk-card uk-card-default uk-card-body uk-card-small">Item 4</div>
            </div>
        </div>
    </div>
    <div>
        <h4>Group 2</h4>
        <div uk-sortable="group: sortable-group">
            <div class="uk-margin">
                <div class="uk-card uk-card-default uk-card-body uk-card-small">Item 1</div>
            </div>
            <div class="uk-margin">
                <div class="uk-card uk-card-default uk-card-body uk-card-small">Item 2</div>
            </div>
            <div class="uk-margin">
                <div class="uk-card uk-card-default uk-card-body uk-card-small">Item 3</div>
            </div>
            <div class="uk-margin">
                <div class="uk-card uk-card-default uk-card-body uk-card-small">Item 4</div>
            </div>
        </div>
    </div>
    <div>
        <h4>Empty Group</h4>
        <div uk-sortable="group: sortable-group">
    </div>
</div>



To be able to sort items from one list to another, you can group them by adding the group: GROUP-NAME option to the uk-sortable attribute on each list.

<div uk-sortable="group: my-group">
    <div></div>
</div>

<div uk-sortable="group: my-group">
    <div></div>
</div>
PREVIEW
MARKUP
Group 1
Item 1
Item 2
Item 3
Item 4
Group 2
Item 1
Item 2
Item 3
Item 4
Empty Group


<ul class="uk-nav uk-nav-default uk-width-medium" uk-sortable="cls-custom: uk-box-shadow-small uk-flex uk-flex-middle uk-background">
    <li class="uk-active"><a href="#">Active</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
</ul>



Custom class
You can also apply one or more custom classes to items when they are being dragged. To do so, add the cls-custom: MY-CLASS option to the attribute.

<ul uk-sortable="cls-custom: my-class">...</ul>
NOTE In this example, we are using a nav from the Nav component. When dragging an item it will get a box-shadow and background.

PREVIEW
MARKUP
Active
Item
Item
Item
Item
Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
group	String	''	The group
animation	Number	150	The animation duration.
threshold	Number	10	Mouse move threshold before dragging starts.
cls-item	String	uk-sortable-item	The item class.
cls-placeholder	String	uk-sortable-placeholder	The placeholder class.
cls-drag	String	uk-sortable-drag	The ghost class.
cls-drag-state	String	uk-sortable-dragging	The body's dragging class.
cls-base	String	uk-sortable	The list's class.
cls-no-drag	String	uk-sortable-nodrag	Disable dragging on elements with this class.
cls-empty	String	uk-sortable-empty	The empty list class.
cls-custom	String	''	The ghost's custom class.
handle	String	false	The handle selector.
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.sortable(element, options);
Events
The following events will be triggered on elements with this component attached:

NAME	DESCRIPTION
start	Fires after dragging starts.
stop	Fires after dragging stops.
moved	Fires after an element has been moved.
added	Fires after an element has been added.
removed	Fires after an element has been removed.
