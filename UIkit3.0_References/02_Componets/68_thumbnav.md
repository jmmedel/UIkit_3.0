

Thumbnav
Create a flexible thumbnail navigation.

Usage
To create a navigation with thumbnails, use the following classes. This component is built with Flexbox. So to align a thumbnav, you can use Flex component.

CLASS	DESCRIPTION
.uk-thumbnav	Add this class to a <ul> element to define the Thumbnav component. Nest your thumbnail images inside <a> elements within the list.
.uk-active	Add this class to a list item to apply an active state.
<ul class="uk-thumbnav">
    <li class="uk-active"><a href=""><img src="" alt=""></a></li>
    <li><a href=""><img src="" alt=""></a></li>
</ul>
NOTE For a better layout, if items should wrap into the next row, add the uk-margin attribute from the Margin component.

PREVIEW
MARKUP



Vertical alignment
The thumbnav can also be displayed vertically. Just add the .uk-thumbnav-vertical modifier.

<ul class="uk-thumbnav uk-thumbnav-vertical">...</ul>
PREVIEW
MARKUP



Position as overlay
To position the thumbnav on top of an element or the Slideshow component for example,, add one of the .uk-position-* classes from the Position component to a div element wrapping the thumbnav. To create a position context on the container, add the .uk-position-relative class.

<div class="uk-position-relative">

    <!-- The element which is wrapped goes here -->

    <div class="uk-position-bottom-center uk-position-small">
        <ul class="uk-thumbnav">...</ul>
    </div>

</div>
PREVIEW
MARKUP

