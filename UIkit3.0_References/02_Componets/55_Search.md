Search
Easily create a nice looking search.

Usage
The Search component consists of a search form and the search input itself.

CLASS/ATTRIBUTE	DESCRIPTION
.uk-search	Add this class to a container element to define the Search component.
.uk-search-input	Add this class to an <input> element to create the search field.
<form class="uk-search">
    <input class="uk-search-input" type="search" placeholder="">
</form>
By default, the search has no additional styling. In this example we are using the .uk-search-default modifier.

PREVIEW
MARKUP

Search...
Search icon
To create a search icon, add the uk-search-icon attribute to a <span> element. To change the alignment, add the .uk-search-icon-flip class.

<form class="uk-search uk-search-default">
    <span uk-search-icon></span>
    <input class="uk-search-input" type="search" placeholder="">
</form>
PREVIEW
MARKUP

Search...
 
Search...
Clickable
To enable an action, use an <a> or <button> element to create the icon.

<form class="uk-search uk-search-default">
    <a href="" uk-search-icon></a>
    <input class="uk-search-input" type="search" placeholder="">
</form>
PREVIEW
MARKUP

Search...
 
Search...
Default modifier
To apply the default search styling, add the .uk-search-default class.

<form class="uk-search uk-search-default">...</form>
PREVIEW
MARKUP

Search...
Large modifier
To increase the size of the search, for example when creating an overlay search, add the .uk-search-large class.

<form class="uk-search uk-search-large">...</form>
PREVIEW
MARKUP

Search...
Navbar modifier
A search can be used inside a navbar from the Navbar component. Just add the .uk-search-navbar class.

<form class="uk-search uk-search-navbar">...</form>
PREVIEW
MARKUP

Search...
Toggle
To apply a hover state to the search icon when using an <a> or <button> element, add the .uk-search-toggle class. To create the search icon itself, add the uk-search-icon attribute.

<a class="uk-search-toggle" href="" uk-search-icon></a>
PREVIEW
MARKUP
Search in navbar
The search icon can be used as a toggle to open the search inside a navbar – as an overlay, drop or dropdown – or outside in a modal. Just add the .uk-navbar-toggle class to the icon.

<div class="uk-navbar-container" uk-navbar>
    <div class="uk-navbar-left">
        <a class="uk-navbar-toggle" uk-search-icon uk-toggle href=""></a>
    </div>
</div>
Overlay
PREVIEW
MARKUP
Logo
ACTIVE
ITEM
Drop
PREVIEW
MARKUP
Logo
ACTIVE
ITEM
Dropdown
PREVIEW
MARKUP
Logo
ACTIVE
ITEM
Modal
PREVIEW
MARKUP
Logo
ACTIVE
ITEM