

Off-canvas
Create an off-canvas sidebar that slides in and out of the page, which is perfect for creating mobile navigations.

Usage
To apply this component, add the uk-offcanvas attribute to a parent <div> element and use the following classes.

CLASS	DESCRIPTION
.uk-offcanvas-bar	Add this class to a child <div> element.
.uk-offcanvas-close	Add this class and the uk-close attribute to an <a> or <button> element to create a close button and enable its functionality.
You can use any element to toggle an off-canvas sidebar. To enable the necessary JavaScript, add the uk-toggle attribute. An <a> element needs to be linked to the id of the off-canvas container. If you are using another element, like a button, just add the uk-toggle="target: #ID" attribute to target the id of the off-canvas container.

<body>

    <!-- This is a button toggling the off-canvas -->
    <button uk-toggle="target: #my-id" type="button"></button>

    <!-- This is an anchor toggling the off-canvas -->
    <a href="#my-id" uk-toggle></a>

    <!-- This is the off-canvas -->
    <div id="my-id" uk-offcanvas>
        <div class="uk-offcanvas-bar">

            <button class="uk-offcanvas-close" type="button" uk-close></button>

        </div>
    </div>

</body>
PREVIEW
MARKUP
OPEN Open
Overlay
To add an overlay, blanking out the page, add the overlay: true parameter to the uk-offcanvas attribute.

<div id="my-id" uk-offcanvas="overlay: true">...</div>
PREVIEW
MARKUP
OPEN
Flip modifier
Add the flip: true parameter to the uk-offcanvas attribute to adjust its alignment, so that it slides in from the right.

<div id="my-id" uk-offcanvas="flip: true">...</div>
PREVIEW
MARKUP
OPEN
Animation modes
By default, the off-canvas slides in. But you can actually choose between different animation modes for the off-canvas' entrance. Just add one of the following attributes.

PARAMETER	DESCRIPTION
mode: slide	The off-canvas slides out and overlays the content. This is the default mode.
mode: push	The off-canvas slides out and pushes the site.
mode: reveal	The off-canvas slides out and reveals its content while pushing the site.
mode: none	The off-canvas appears and overlays the content without an animation.
<div id="my-id" uk-offcanvas="mode: push">...</div>
PREVIEW
MARKUP
SLIDE  PUSH  REVEAL  NONE
Nav in Off-canvas
You can use the Nav component inside an off-canvas to create a mobile navigation.

<div id="my-id" uk-offcanvas>
    <div class="uk-offcanvas-bar">
        <ul class="uk-nav uk-nav-default">...</ul>
    </div>
</div>
PREVIEW
MARKUP
PRIMARY NAV  DEFAULT NAV
Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
mode	String	slide	Off-canvas animation mode: slide, reveal, push or none.
flip	Boolean	false	Flip off-canvas to the right side.
overlay	Boolean	false	Display the off-canvas together with an overlay.
esc-close	Boolean	true	Close the off-canvas when the Esc key is pressed.
bg-close	Boolean	true	Close the off-canvas when the background is clicked.
container	String	true	Define a target container via a selector to specify where the off-canvas should be appended in the DOM. Setting it to false will prevent this behavior.
mode is the Primary option and its key may be omitted, if it's the only option in the attribute value.

<span uk-offcanvas="push"></span>
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.offcanvas(element, options);
Events
The following events will be triggered on elements with this component attached:

NAME	DESCRIPTION
beforeshow	Fires before an item is shown.
show	Fires after an item is shown.
shown	Fires after the item's show animation has completed.
beforehide	Fires before an item is hidden.
hide	Fires after an item's hide animation has started.
hidden	Fires after an item is hidden.
Methods
The following methods are available for the component:

Show
UIkit.offcanvas(element).show();
Shows the Offcanvas.

Hide
UIkit.offcanvas(element).hide();
Hides the Offcanvas.