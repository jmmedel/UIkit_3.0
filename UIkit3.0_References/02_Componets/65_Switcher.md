
Switcher
Dynamically transition through different content panes.

Usage
The Switcher component consists of a number of toggles and their related content items. Add the uk-switcher attribute to the element which contains the toggles. Add the .uk-switcher class to the element containing the content items.

By default, the element with the .uk-switcher class has to succeed the toggle directly in order for the switcher to function. If you need it to be nested in another element, for example when using a grid, add the connect: SELECTOR option to the uk-switcher attribute and select the element containing the items for switching.

Typically, the switcher toggles are styled through other components, some of which will be shown here.

<!-- This is the nav containing the toggling elements -->
<ul uk-switcher>
    <li><a href="#"></a></li>
</ul>

<!-- This is the container of the content items -->
<ul class="uk-switcher">
    <li></li>
</ul>
In this example we are using the Subnav component.

PREVIEW
MARKUP
ITEM
ITEM
ITEM
Hello!

<ul class="uk-subnav uk-subnav-pill" uk-switcher>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
</ul>

<ul class="uk-switcher uk-margin">
    <li>Hello!</li>
    <li>Hello again!</li>
    <li>Bazinga!</li>
</ul>




Navigation controls
In some cases you want to switch to another content section from within the active content. This is possible using the uk-switcher-item attribute. To target the items, you need to set the attribute to the number of the respective content item.

Setting the attribute to next and previous will switch to the adjacent items.

<ul class="uk-switcher uk-margin">
    <li><a href="#" uk-switcher-item="0"></a></li>
    <li><a href="#" uk-switcher-item="1"></a></li>
    <li><a href="#" uk-switcher-item="next"></a></li>
    <li><a href="#" uk-switcher-item="previous"></a></li>
</ul>
PREVIEW
MARKUP
ITEM
ITEM
ITEM


<ul class="uk-subnav uk-subnav-pill" uk-switcher>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
</ul>
<ul class="uk-switcher uk-margin">
    <li>Hello! <a href="#" uk-switcher-item="2">Switch to item 3</a></li>
    <li>Hello again! <a href="#" uk-switcher-item="next">Next item</a></li>
    <li>Bazinga! <a href="#" uk-switcher-item="previous">Previous item</a></li>
</ul>




Hello! Switch to item 3
Connect multiple containers
It is also possible to connect multiple content containers. Just add the connect parameter to the uk-switcher attribute and use a selector that applies to all items.

<!-- This is the nav containing the toggling elements -->
<ul uk-switcher="connect: .my-class">...</ul>

<!-- These are the containers of the content items -->
<ul class="uk-switcher my-class">...</ul>

<ul class="uk-switcher my-class">...</ul>
PREVIEW
MARKUP
ACTIVE
ITEM
ITEM
Container 1
Hello!
Container 2
Hello! The first item.



<ul class="uk-subnav uk-subnav-pill" uk-switcher="connect: .switcher-container">
    <li><a href="#">Active</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
</ul>

<h4>Container 1</h4>

<ul class="uk-switcher switcher-container uk-margin">
    <li>Hello!</li>
    <li>Hello again!</li>
    <li>Bazinga!</li>
</ul>

<h4>Container 2</h4>

<ul class="uk-switcher switcher-container uk-margin">
    <li>Hello! The first item.</li>
    <li>Hello again! The second item.</li>
    <li>Bazinga! The third item.</li>
</ul>




Animations
You can apply all animations from the Animation component to switcher items. To do so, add the animation parameter with the relevant class to the uk-switcher attribute.

<ul uk-switcher="animation: uk-animation-fade">...</ul>
PREVIEW
MARKUP
ITEM
ITEM
ITEM
Hello!


<ul class="uk-subnav uk-subnav-pill" uk-switcher="animation: uk-animation-fade">
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
</ul>

<ul class="uk-switcher uk-margin">
    <li>Hello!</li>
    <li>Hello again!</li>
    <li>Bazinga!</li>
</ul>



Multiple animations
You can also apply multiple animations from the Animation component. That way you can add different in and out animations.

<ul uk-switcher="animation: uk-animation-slide-left-medium, uk-animation-slide-right-medium">...</ul>
PREVIEW
MARKUP
ITEM
ITEM
ITEM
Hello!

<ul class="uk-subnav uk-subnav-pill" uk-switcher="animation: uk-animation-slide-left-medium, uk-animation-slide-right-medium">
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
</ul>

<ul class="uk-switcher uk-margin">
    <li>Hello!</li>
    <li>Hello again!</li>
    <li>Bazinga!</li>
</ul>



Switcher and subnav
The switcher is easily applied to the Subnav component.

<!-- This is the subnav containing the toggling elements -->
<ul class="uk-subnav uk-subnav-pill" uk-switcher>...</ul>

<!-- This is the container of the content items -->
<ul class="uk-switcher"></ul>
PREVIEW
MARKUP
ITEM
ITEM
ITEM
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Switcher and tab
As an exception to the rule, add the uk-tab attribute instead of uk-switcher to the tabbed navigation to combine the switcher with the Tab component.

<!-- This is the subnav containing the toggling elements -->
<ul uk-tab>...</ul>

<!-- This is the container of the content items -->
<ul class="uk-switcher">...</ul>
PREVIEW
MARKUP
ITEM
ITEM
ITEM
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Vertical tabs
Use the Grid and Width components to display content correctly with a vertical tabbed navigation.



<ul class="uk-subnav uk-subnav-pill" uk-switcher>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
</ul>

<ul class="uk-switcher uk-margin">
    <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</li>
    <li>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</li>
    <li>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur, sed do eiusmod.</li>
</ul>


<div uk-grid>
    <div class="uk-width-auto">
        <ul class="uk-tab-left" uk-tab="connect: #my-id">...</ul>
    </div>
    <div class="uk-width-expand">
        <ul id="my-id" class="uk-switcher">...</ul>
    </div>
</div>
PREVIEW
MARKUP
ACTIVE
ITEM
ITEM
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
ACTIVE
ITEM
ITEM
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Switcher and button
The switcher can also be applied to buttons or button groups from the Button component. Just add the switcher attribute to a block around a group of buttons or to the element with the .uk-button-group class.

<!-- This is a switcher using a number of buttons -->
<div uk-switcher>
    <button class="uk-button uk-button-default" type="button"></button>
    <button class="uk-button uk-button-default" type="button"></button>
</div>

<ul class="uk-switcher">...</ul>


<ul uk-tab>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
</ul>

<ul class="uk-switcher uk-margin">
    <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</li>
    <li>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</li>
    <li>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur, sed do eiusmod.</li>
</ul>



PREVIEW
MARKUP
ITEM  ITEM  ITEM
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Switcher and nav
To apply the switcher to the Nav component, add the uk-switcher attribute to the nav <ul> element. Use the Grid and Width components to arrange nav and content in a grid layout.

<div uk-grid>
    <div class="uk-width-small">
        <ul class="uk-nav uk-nav-default" uk-switcher="connect: #my-id">...</ul>
    </div>
    <div class="uk-width-expand">
        <ul id="my-id" class="uk-switcher">...</ul>
    </div>
</div>
PREVIEW
MARKUP
Active
Item
Item
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
connect	CSS selector	~.uk-switcher	Related items container. By default succeeding elements with class 'uk-switcher'.
toggle	CSS selector	> *	The toggle selector, which triggers content switching on click.
active	Number	0	Active index on init. Providing a negative number indicates a position starting from the end of the set.
animation	String	false	The space separated names of animations to use. Comma separate for animation out.
duration	Number	200	The animation duration.
swiping	Boolean	true	Use swiping.
connect is the Primary option and its key may be omitted, if it's the only option in the attribute value.



<div class="uk-child-width-1-2@s" uk-grid>
    <div>
        <div uk-grid>
            <div class="uk-width-auto@m">
                <ul class="uk-tab-left" uk-tab="connect: #component-tab-left; animation: uk-animation-fade">
                    <li><a href="#">Active</a></li>
                    <li><a href="#">Item</a></li>
                    <li><a href="#">Item</a></li>
                </ul>
            </div>
            <div class="uk-width-expand@m">
                <ul id="component-tab-left" class="uk-switcher">
                    <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</li>
                    <li>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</li>
                    <li>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur, sed do eiusmod.</li>
                </ul>
            </div>
        </div>
    </div>
    <div>
        <div uk-grid>
            <div class="uk-width-auto@m uk-flex-last@m">
                <ul class="uk-tab-right" uk-tab="connect: #component-tab-right; animation: uk-animation-fade">
                    <li><a href="#">Active</a></li>
                    <li><a href="#">Item</a></li>
                    <li><a href="#">Item</a></li>
                </ul>
            </div>
            <div class="uk-width-expand@m">
                <ul id="component-tab-right" class="uk-switcher">
                    <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</li>
                    <li>Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</li>
                    <li>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur, sed do eiusmod.</li>
                </ul>
            </div>
        </div>
    </div>
</div>



<span uk-switcher=".switcher-container"></span>
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.switcher(element, options);
Events
The following events will be triggered on the connected items of the elements with this component attached:

NAME	DESCRIPTION
beforeshow	Fires before an item is shown. Can prevent showing by returning false.
show	Fires after an item is shown.
shown	Fires after the item's show animation has completed.
beforehide	Fires before an item is hidden. Can prevent hiding by returning false.
hide	Fires after an item's hide animation has started.
hidden	Fires after an item is hidden.
Methods
The following methods are available for the component:

Show
UIkit.switcher(element).show(index);
Shows the Switcher item with given index.

NAME	TYPE	DEFAULT	DESCRIPTION
index	String, Integer, Node	0	Switcher item to show. 0 based index.
