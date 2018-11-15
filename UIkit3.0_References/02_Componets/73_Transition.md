

Transition
Create smooth transitions between two states when hovering an element.

Usage
To apply this component, add the .uk-transition-toggle class to a parent element. This will trigger the transition when the element is hovered. Also add tabindex="0" to make the transition accessable through keyboard navigation.

Add one of the .uk-transition-* classes to the element itself to apply the actual effect.

This component is mostly used in combination with the Overlay component as elements are transitioned from invisible to visible state. To place the overlay on top of another element, like an image, use the Position component.

<div class="uk-transition-toggle" tabindex="0">
    <div class="uk-transition-fade"></div>
</div>
CLASS	DESCRIPTION
.uk-transition-fade	Lets the element fade in
.uk-transition-scale-up
.uk-transition-scale-down	The element scales up or down.
.uk-transition-slide-top
.uk-transition-slide-bottom
.uk-transition-slide-left
.uk-transition-slide-right	Lets the element slide in from the top
.uk-transition-slide-top-small
.uk-transition-slide-bottom-small
.uk-transition-slide-left-small
.uk-transition-slide-right-small	The element slides in from the top, bottom, left or right with a smaller distance.
.uk-transition-slide-top-medium
.uk-transition-slide-bottom-medium
.uk-transition-slide-left-medium
.uk-transition-slide-right-medium	The element slides in from the top, bottom, left or right with a medium distance.
PREVIEW
MARKUP

Fade

Fade


Bottom

Bottom


Icon

 
2 Images


Scale Up Image


Headline
Subheadline
Small Top + Bottom
