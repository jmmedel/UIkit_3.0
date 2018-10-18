

Height
Define the height of elements depending on the viewport or match the heights of different elements.

UIkit's Height component offers three options to set heights: using simple fixed height utility classes, depending on the viewport or by matching the heights of different elements.

Usage
UIkit provides a number of useful classes to alter an element's height.

CLASS	DESCRIPTION
.uk-height-1-1	This class applies a height of 100%. This only works if the parent element has a set height.
.uk-height-small
.uk-height-max-small	These classes apply a height or max-height of 150px.
.uk-height-medium
.uk-height-max-medium	These classes apply a height or max-height of 300px.
.uk-height-large
.uk-height-max-large	These classes apply a height or max-height of 450px.
<div class="uk-height-small"></div>
PREVIEW
MARKUP
Small
Medium
Large
Viewport height
Add the uk-height-viewport attribute to create a container that fills the height of the entire viewport. You can change the height behavior by adding the offset-top, offset-bottom or expand option to the attribute. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
offset-top	Boolean	false	Subtracts the element's top offset from its height.
offset-bottom	Boolean, Number, Pixel	false	Subtracts the height (true) of the sibling that immediately follows the element, the given percentage (Number), Pixel (px) value from element's own height or the given element's height.
expand	Boolean	true	Expands the element's height to make a short page fill the viewport.
min-height	Number	0	Sets a minimum height. Useful if all children are positioned absolute.
<div uk-height-viewport></div>

<div uk-height-viewport="offset-top: true"></div>

<div uk-height-viewport="offset-bottom: 20"></div>

<div uk-height-viewport="expand: true"></div>

<div uk-height-viewport="min-height: 300"></div>
You can view examples in the tests for Height Viewport and Height Expand.

Match height
To expand all children of a container to the same height regardless of their content, for example inside a grid, add the uk-height-match attribute. You can change the height matching behavior by setting the target or row option to the attribute. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
target	String	> *	Elements that should match.
row	Boolean	true	By default only items in the same row will be matched. For example, once grid columns extend to a width of 100%, their heights will no longer be matched. This makes sense, for example, if they stack vertically in narrower viewports.
<div uk-height-match>
    <div></div>
    <div></div>
</div>
target is the Primary option, and its key may be omitted if it's the only option in the attribute value.

<span uk-height-match=".my-class"></span>
Match cards
You can also target and match specific elements inside the container, like cards. Just add the target: SELECTOR option to the attribute.

<div uk-grid uk-height-match="target: SELECTOR">...</div>
PREVIEW
MARKUP
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Lorem Ipsum
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
Lorem Ipsum
Match all
If your grid wraps into multiple rows, only grid columns within the same row are matched. To match grid columns across all rows, just add the row: false option to the attribute.

<div uk-grid uk-height-match="row: false">...</div>
PREVIEW
MARKUP
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Lorem Ipsum
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
Lorem Ipsum
Component options
The table below lists the available settings of the uk-height-match attribute. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
target	CSS selector	> *	Elements that should match. By default, direct children will match.
row	Boolean	true	If your targets wrap into multiple rows, only grid columns within the same row are matched.
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.heightMatch(element, options);


