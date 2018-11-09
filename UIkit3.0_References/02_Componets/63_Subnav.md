

Subnav
Defines different styles for a sub navigation.

Usage
To apply this component, use the following classes. To align a subnav, for example to horizontally center it, you can use the Flex component.

CLASS	DESCRIPTION
.uk-subnav	Add this class to a <ul> element to define the Subnav component. Use <a> elements as nav items within the list.
.uk-active	Add this class to a list item to apply an active state.
To add list items without a link, use a <span> element instead of an <a>. Alternatively, disable an <a> element by adding the .uk-disabled class to the <li> element and remove the href attribute from the anchor to make it inaccessible through keyboard navigation.

<ul class="uk-subnav">
    <li class="uk-active"><a href=""></a></li>
    <li><a href=""></a></li>
    <li><span></span></li>
</ul>
PREVIEW
MARKUP
ACTIVE
ITEM
ITEM
DISABLED
NOTE For a better layout, if items should wrap into the next row, add the uk-margin attribute from the Margin component.

Divider modifier
Add the .uk-subnav-divider class to separate menu items with lines.

<ul class="uk-subnav uk-subnav-divider">...</ul>
PREVIEW
MARKUP
ACTIVE
ITEM
ITEM
Pill modifier
Add the .uk-subnav-pill class to highlight the active menu item with a background.

<ul class="uk-subnav uk-subnav-pill">...</ul>
PREVIEW
MARKUP
ACTIVE
ITEM
ITEM
Subnav with Dropdown
You can also use a dropdown from the Dropdown component with a subnav.

<ul class="uk-subnav">
    <li>
        <a href=""></a>
        <div uk-dropdown="mode: click;"></div>
    </li>
</ul>
PREVIEW
MARKUP
ACTIVE
ITEM
MORE 
