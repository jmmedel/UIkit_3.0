
Position
A collection of utility classes to position content.

Usage
To apply this component, add one of the .uk-position-* classes to a block element. When using this component to place content on top of an image, add the .uk-inline class from the Utility component to a container element around the image and the element to create a position context.

NOTE This is often used to position an overlay from the Overlay component. Use the .uk-light or .uk-dark class from the Inverse component to apply a light or dark color for better visibility.

CLASS	DESCRIPTION
.uk-position-top	Positions the element at the top.
.uk-position-left	Positions the element at the left.
.uk-position-right	Positions the element at the right.
.uk-position-bottom	Positions the element at the bottom.
<div class="uk-inline">

    <!-- Place any content, like an image, here -->

    <div class="uk-position-center"></div>

</div>
PREVIEW
MARKUP
TopBottomLeftRight
X and Y directions
You can also apply more specific positions that won't spread over one side of the parent container by adding one of the following classes.

CLASS	DESCRIPTION
.uk-position-top-left	Positions the element at the top left.
.uk-position-top-center	Positions the element at the top center.
.uk-position-top-right	Positions the element at the top right.
.uk-position-center	Positions the element vertically centered in the middle.
.uk-position-center-left	Positions the element vertically centered on the left.
.uk-position-center-right	Positions the element vertically centered on the right.
.uk-position-bottom-left	Positions the element at the bottom left.
.uk-position-bottom-center	Positions the element at the bottom center.
.uk-position-bottom-right	Positions the element at the bottom right.
<div class="uk-position-top-right"></div>
PREVIEW
MARKUP
Top LeftTop CenterTop RightCenter LeftCenterCenter RightBottom LeftBottom CenterBottom Right
Cover
If you want a position element to cover its container, just add the .uk-position-cover class.

<div class="uk-position-cover"></div>
PREVIEW
MARKUP
Cover
Outside
There are two classes to center elements outside on the left and right of the parent container. This is useful to position the Slidenav component outside of an Slideshow or Slider component.

CLASS	DESCRIPTION
.uk-position-center-left-out	Positions the element vertically centered outside on the left.
.uk-position-center-right-out	Positions the element vertically centered outside on the right.
NOTE Once the outside positioned element sticks out of the viewport to the right, it will cause a horizontal scrollbar. Use the Visibility component to hide the outside positioned element on a smaller viewports and show an inside positioned element instead.

<div class="uk-position-center-left-out"></div>
PREVIEW
MARKUP
OutOut
Small modifier
To apply a small margin to positioned elements, add the .uk-position-small class.

<div class="uk-position-small uk-position-center"></div>
PREVIEW
MARKUP
Top LeftTop CenterTop RightCenter LeftCenterCenter RightBottom LeftBottom CenterBottom Right TopBottomLeftRight Cover
OutOut
Medium modifier
To apply a medium margin to positioned elements, add the .uk-position-medium class.

<div class="uk-position-medium uk-position-center"></div>
PREVIEW
MARKUP
Top LeftTop CenterTop RightCenter LeftCenterCenter RightBottom LeftBottom CenterBottom Right TopBottomLeftRight Cover
OutOut
Large modifier
To apply a large margin to positioned elements, add the .uk-position-large class.

<div class="uk-position-large uk-position-center"></div>
PREVIEW
MARKUP
Top LeftTop CenterTop RightCenter LeftCenterCenter RightBottom LeftBottom CenterBottom Right TopBottomLeftRight Cover
OutOut
Utility classes
This component features a number of general position utility classes:

CLASS	DESCRIPTION
.uk-position-relative	Add this class to apply relative positioning.
.uk-position-absolute	Add this class to apply absolute positioning.
.uk-position-fixed	Add this class to apply fixed positioning.
.uk-position-z-index	Add this class to apply a z-index of 1.
