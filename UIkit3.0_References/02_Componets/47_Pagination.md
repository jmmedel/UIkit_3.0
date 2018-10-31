

Pagination
Easily create a nice looking pagination to navigate through pages.

Usage
The Pagination component consists of button-like styled links, that are aligned side by side in a horizontal list.

CLASS	DESCRIPTION
.uk-pagination	Add this class to a <ul> element to define the Pagination component. Use <a> elements as pagination items within the list.
.uk-active	Add this class to a list item to apply an active state and use a <span> instead of an <a> element.
.uk-disabled	Add this class to a list item to apply a disabled state and use a <span> instead of an <a> element.
<ul class="uk-pagination">
    <li><a href=""></a></li>
    <li class="uk-active"><span></span></li>
    <li class="uk-disabled"><span></span></li>
</ul>
PREVIEW
MARKUP
1
...
4
5
6
7
8
9
10
...
20
Alignment
The pagination component utilizes flexbox, so navigations can easily be aligned with the Flex component.

<ul class="uk-pagination uk-flex-center">...</ul>
PREVIEW
MARKUP
1
...
5
6
7
8
1
...
5
6
7
8
Previous and next
To apply a previous and next button, add the uk-pagination-previous or uk-pagination-next attribute to a <span> element inside a pagination item.

<ul class="uk-pagination">
    <li><a href=""><span uk-pagination-previous></span></a></li>
    <li><a href=""><span uk-pagination-next></span></a></li>
</ul>
PREVIEW
MARKUP
 Previous
Next 
