
Sticky
Make elements remain at the top of the viewport, like a sticky navigation.

Usage
To create an element that remains at the top of the viewport when scrolling down the site, add the uk-sticky attribute to that element.

<div uk-sticky></div>
PREVIEW
MARKUP
Stick to the top
NOTE Example elements on this page are only sticky until you scroll down to the next heading and disappear afterwards. This was done so as not to clutter your screen with all variations of sticky containers.

Offset
You can position the element below the viewport edge. Add the offset attribute and the distance in pixels.

<div uk-sticky="offset: 100"></div>
PREVIEW
MARKUP
Stick 100px below the top
Top
To apply the sticky behavior with a delay, add the top attribute, which can be defined either by a number representing the offset in pixels, but also viewport height or a CSS selector.

<!-- Sticks after 100px of scrolling -->
<div uk-sticky="top: 100"></div>

<!-- Sticks after 100vh -->
<div uk-sticky="top: 100vh"></div>

<!-- Sticks to the top of the container -->
<div id="my-id">
    <div uk-sticky="top: #my-id"></div>
</div>
PREVIEW
MARKUP
Stick to the top but only after 200px scrolling
Stick to the top but below the box
Animation
Add an animation from the Animation component in order to have the sticky element reappear smoothly.

<div uk-sticky="animation: uk-animation-slide-top"></div>
PREVIEW
MARKUP
Animation Slide Top
Sticky on scroll up
You can make the sticky element show only when scrolling up to save space. Together with an animation, this makes for a very smooth experience.

<div uk-sticky="show-on-up: true"></div>
PREVIEW
MARKUP
Slide in on scroll up
Bottom
Bind the sticky behavior to a specific element, so that it disappears after scrolling past that point of the page.

<!-- Sticks until the bottom of its parent container -->
<div>
    <div uk-sticky="bottom: true"></div>
</div>

<!-- Sticks until the second container -->
<div uk-sticky="bottom: #my-id"></div>
<div id="my-id"></div>
PREVIEW
MARKUP
Stick until the bottom of its parent container
Stick until the next headline
Some Headline
Responsive
It's possible to disable the sticky behavior for different devices widths by applying the media option to the attribute and adding the appropriate viewport width. Add a number in pixel, for example media: 640, or a breakpoint, for example media: @m. The element will be sticky from the specified viewport width and upwards, but not below.

<div uk-sticky="media: 640"></div>
Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
top	Number, viewport height, CSS selector	0	The top offset from where the element should be stick.
bottom	Boolean, CSS selector	false	The bottom offset until the element should stick. (true: parent element, prefixed with '!' a parent selector)
offset	Number	0	The offset the Sticky should be fixed to.
animation	String	false	The animation to use when the element becomes sticky.
cls-active	String	uk-active	The active class.
cls-inactive	String	''	The inactive class.
width-element	CSS selector	false	The element the Sticky should get its width from in active mode.
show-on-up	Boolean	false	Only show sticky element when scrolling up.
media	Integer, String	false	Condition for the active status - a width as integer (e.g. 640) or a breakpoint (e.g. @s, @m, @l, @xl) or any valid media query (e.g. (min-width: 900px)).
target-offset	Boolean, Number	false	Initially make sure that the Sticky is not over a targeted element via location hash.
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.sticky(element, options);
Events
The following events will be triggered on elements with this component attached:

NAME	DESCRIPTION
active	Fires after the element becomes sticky.
inactive	Fires after the element is no longer sticky.
