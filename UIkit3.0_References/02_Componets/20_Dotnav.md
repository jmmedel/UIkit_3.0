
Dotnav
Create a dot navigation to operate slideshows or to scroll to different page sections.

Usage
To create a navigation with dots, use the following classes. This component is built with Flexbox. So to align a dotnav, you can use Flex component.

CLASS	DESCRIPTION
.uk-dotnav	Add this class to a <ul> element to define the Dotnav component. Use <a> elements as nav items within the list.
.uk-active	Add this class to a list item to apply an active state.
<ul class="uk-dotnav">
    <li class="uk-active"><a href=""></a></li>
    <li><a href=""></a></li>
</ul>
PREVIEW
MARKUP



Item 1
Item 2
Item 3
Item 4
Item 5

<ul class="uk-dotnav">
    <li class="uk-active"><a href="#">Item 1</a></li>
    <li><a href="#">Item 2</a></li>
    <li><a href="#">Item 3</a></li>
    <li><a href="#">Item 4</a></li>
    <li><a href="#">Item 5</a></li>
</ul>


Vertical alignment
The dotnav can also be displayed vertically. Just add the .uk-dotnav-vertical modifier.

<ul class="uk-dotnav uk-dotnav-vertical">...</ul>
PREVIEW
MARKUP
Item 1
Item 2
Item 3
Item 4
Item 5

Position as overlay
To position the dotnav on top of an element or the Slideshow component for example, add one of the .uk-position-* classes from the Position component to a div element wrapping the dotnav. To create a position context on the container, add the .uk-position-relative class.

Use the .uk-light or .uk-dark class from the Inverse component to apply a light or dark color for better visibility.

<div class="uk-position-relative uk-light">

    <!-- The element which is wrapped goes here -->

    <div class="uk-position-bottom-center uk-position-small">
        <ul class="uk-dotnav">...</ul>
    </div>

</div>
PREVIEW
MARKUP


<div class="uk-position-relative uk-light" uk-slideshow>

    <ul class="uk-slideshow-items">
        <li>
            <img src="images/photo.jpg" alt="" uk-cover>
        </li>
        <li>
            <img src="images/dark.jpg" alt="" uk-cover>
        </li>
        <li>
            <img src="images/size1.jpg" alt="" uk-cover>
        </li>
    </ul>

    <div class="uk-position-bottom-center uk-position-small">
        <ul class="uk-dotnav">
            <li uk-slideshow-item="0"><a href="#">Item 1</a></li>
            <li uk-slideshow-item="1"><a href="#">Item 2</a></li>
            <li uk-slideshow-item="2"><a href="#">Item 3</a></li>
        </ul>
    </div>

</div>


Item 1
Item 2
Item 3
Vertically center in viewport
The dotnav can also be centered vertically inside your viewport by adding the .uk-position-center-right and .uk-position-fixed classes from the Position component. This is useful for typical onepage websites.

<div class="uk-position-center-right uk-position-medium uk-position-fixed">
    <ul class="uk-dotnav uk-dotnav-vertical">...</ul>
</div>
