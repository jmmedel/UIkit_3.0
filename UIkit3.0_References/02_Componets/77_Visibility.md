

Visibility
Use responsive visibility classes to display or hide elements on different devices.

Usage
Add one of these classes to hide an element.

CLASS	DESCRIPTION
.uk-hidden	Hides the element on any device. This is more of a legacy class. The recommended way to do this, is to use the hidden attribute.
.uk-invisible	Hides the element without removing it from the document flow.
<div hidden></div>

<div class="uk-invisible"></div>
Responsive
This component provides responsive classes to hide or display elements on different viewports.

Hidden
Add one of the .uk-hidden-* classes to hide the element from screens larger than a specified width.

CLASS	DESCRIPTION
uk-hidden@s	Only affects device widths of 640px and larger.
uk-hidden@m	Only affects device widths of 960px and larger.
uk-hidden@l	Only affects device widths of 1200px and larger.
uk-hidden@xl	Only affects device widths of 1600px and larger.
<!-- Hidden on tablets and larger -->
<div class="uk-hidden@m"></div>
NOTE In this example the green elements are hidden on screens that are larger than the defined breakpoint. Resize your browser window to see the effect.

PREVIEW
MARKUP
✔ Small
Small
✔ Medium
Medium
✔ Large
Large
✔ XLarge
XLarge
Visible
Use .uk-visible-* classes to show the element for screens larger than the specified width.

CLASS	DESCRIPTION
uk-visible@s	Only affects device widths of 640px and larger.
uk-visible@m	Only affects device widths of 960px and larger.
uk-visible@l	Only affects device widths of 1200px and larger.
uk-visible@xl	Only affects device widths of 1600px and larger.
<!-- Visible on tablets and larger -->
<div class="uk-visible@m"></div>
NOTE In this example the green elements are displayed on screens that are larger than the defined breakpoint. Resize your browser window to see the effect.

PREVIEW
MARKUP
Small
Medium
Large
XLarge
Show on hover
Use one of the following classes to display elements only when they are being hovered.

CLASS	DESCRIPTION
.uk-visible-toggle	Add this class to any parent element of the element to hide. This enables the toggling on hover.
.uk-hidden-hover	Add this class to the child element to hide the content and remove it from the document flow.
.uk-invisible-hover	Add this class to the child element to hide the content without removing it from the document flow.
<div class="uk-visible-toggle">
    <div class="uk-hidden-hover"></div>
</div>
PREVIEW
MARKUP
Hidden when not hovered
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
Invisible when not hovered
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
Touch
Add the .uk-hidden-touch class to hide elements on touch devices and the .uk-hidden-notouch to hide elements on devices without a touch screen.

<!-- Hidden on touch devices -->
<div class="uk-hidden-touch"></div>

<!-- Hidden on no-touch devices -->
<div class="uk-hidden-notouch"></div>
PREVIEW
MARKUP
✔ Hidden Touch
Hidden Touch
✔ Hidden No-Touch
