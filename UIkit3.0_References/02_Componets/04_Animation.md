

Animation
A collection of smooth animations to use within your page.

Usage
Add one of the .uk-animation-* classes to any element. The animation is shown when the class is added, so usually immediately on page load. To show the animation at another point, for example when the element enters the viewport, you would add the class using JavaScript — with the Scrollspy component for instance. This is what happens in many of UIkit's components that make use of animations. All animations themselves are implemented with CSS, so they do not require JavaScript to play.

CLASS	DESCRIPTION
.uk-animation-fade	The element fades in.
.uk-animation-scale-up
.uk-animation-scale-down	The element fades in and scales up or down.
.uk-animation-slide-top
.uk-animation-slide-bottom .uk-animation-slide-left
.uk-animation-slide-right	The element fades and slides in from the top, bottom, left or right by its own height or width.
.uk-animation-slide-top-small
.uk-animation-slide-bottom-small .uk-animation-slide-left-small
.uk-animation-slide-right-small	The element fades and slides in from the top, bottom, left or right with a smaller distance which is specified by a fixed pixel value.
.uk-animation-slide-top-medium
.uk-animation-slide-bottom-medium .uk-animation-slide-left-medium
.uk-animation-slide-right-medium	The element fades and slides in from the top, bottom, left or right with a medium distance which is specified by a fixed pixel value.
.uk-animation-kenburns	The element scales very slowly up without fading in.
.uk-animation-shake	The element shakes.
<div class="uk-animation-toggle">
    <div class="uk-animation-fade"></div>
</div>
PREVIEW
MARKUP
Fade

Scale Up

Scale Down

Shake

Left

Top

Bottom

Right

Left Small

Top Small

Bottom Small

Right Small

Left Medium

Top Medium

Bottom Medium

Right Medium


<div class="uk-child-width-1-2 uk-child-width-1-4@s uk-grid-match" uk-grid>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-fade">
            <p class="uk-text-center">Fade</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-scale-up">
            <p class="uk-text-center">Scale Up</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-scale-down">
            <p class="uk-text-center">Scale Down</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-shake">
            <p class="uk-text-center">Shake</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-left">
            <p class="uk-text-center">Left</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-top">
            <p class="uk-text-center">Top</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-bottom">
            <p class="uk-text-center">Bottom</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-right">
            <p class="uk-text-center">Right</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-left-small">
            <p class="uk-text-center">Left Small</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-top-small">
            <p class="uk-text-center">Top Small</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-bottom-small">
            <p class="uk-text-center">Bottom Small</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-right-small">
            <p class="uk-text-center">Right Small</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-left-medium">
            <p class="uk-text-center">Left Medium</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-top-medium">
            <p class="uk-text-center">Top Medium</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-bottom-medium">
            <p class="uk-text-center">Bottom Medium</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-right-medium">
            <p class="uk-text-center">Right Medium</p>
        </div>
    </div>
</div>



To apply the hover effect, add the .uk-animation-toggle class on a parent element. This will trigger the animation when the element is hovered.

Reverse modifier
By default, all animations are incoming. To reverse any animation, add the .uk-animation-reverse class.

<div class="uk-animation-fade uk-animation-reverse"></div>
PREVIEW
MARKUP
Fade

Scale Up

Scale Down

Shake

Left

Top

Bottom

Right

Left Small

Top Small

Bottom Small

Right Small

Left Medium

Top Medium

Bottom Medium

Right Medium

Fast modifier


<div class="uk-child-width-1-2 uk-child-width-1-4@s uk-grid-match" uk-grid>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-fade uk-animation-reverse">
            <p class="uk-text-center">Fade</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-scale-up uk-animation-reverse">
            <p class="uk-text-center">Scale Up</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-scale-down uk-animation-reverse">
            <p class="uk-text-center">Scale Down</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-shake uk-animation-reverse">
            <p class="uk-text-center">Shake</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-left uk-animation-reverse">
            <p class="uk-text-center">Left</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-top uk-animation-reverse">
            <p class="uk-text-center">Top</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-bottom uk-animation-reverse">
            <p class="uk-text-center">Bottom</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-right uk-animation-reverse">
            <p class="uk-text-center">Right</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-left-small uk-animation-reverse">
            <p class="uk-text-center">Left Small</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-top-small uk-animation-reverse">
            <p class="uk-text-center">Top Small</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-bottom-small uk-animation-reverse">
            <p class="uk-text-center">Bottom Small</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-right-small uk-animation-reverse">
            <p class="uk-text-center">Right Small</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-left-medium uk-animation-reverse">
            <p class="uk-text-center">Left Medium</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-top-medium uk-animation-reverse">
            <p class="uk-text-center">Top Medium</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-bottom-medium uk-animation-reverse">
            <p class="uk-text-center">Bottom Medium</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-slide-right-medium uk-animation-reverse">
            <p class="uk-text-center">Right Medium</p>
        </div>
    </div>
</div>



To play animations at a faster speed, add the .uk-animation-fast class to the element.

<div class="uk-animation-fade uk-animation-fast"></div>
PREVIEW
MARKUP
Fade

<div class="uk-width-1-3@s">
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-fast uk-animation-fade">
            <p class="uk-text-center">Fade</p>
        </div>
    </div>
</div>




Origin modifiers
By default, scaling animations originate from the center. To modify this behavior, add one of the .uk-transform-origin-* classes from the Utility component.

<div class="uk-animation-scale-up uk-transform-origin-bottom-right"></div>
PREVIEW
MARKUP
Bottom Right

Top Center

Bottom Center


<div class="uk-child-width-1-3@s" uk-grid>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-scale-up uk-transform-origin-bottom-right">
            <p class="uk-text-center">Bottom Right</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-scale-up uk-transform-origin-top-center">
            <p class="uk-text-center">Top Center</p>
        </div>
    </div>
    <div class="uk-animation-toggle">
        <div class="uk-card uk-card-default uk-card-body uk-animation-scale-up uk-transform-origin-bottom-center">
            <p class="uk-text-center">Bottom Center</p>
        </div>
    </div>
</div>


Ken Burns
To add a simple Ken Burns effect, add the .uk-animation-kenburns class to any image. You can also apply the .uk-animation-reverse or one of the .uk-transform-origin-* classes from the Utility component to modify the effect.

<img class="uk-animation-kenburns" src="" alt="">
By default the animation starts on page load. In this example we used the Scrollspy component, to toggle the effect when the image enters the view.

PREVIEW
MARKUP
Example image

<div class="uk-child-width-1-2@s uk-grid-small" uk-grid>
    <div>
        <div class="uk-overflow-hidden">
            <img src="images/dark.jpg" alt="Example image" uk-scrollspy="cls: uk-animation-kenburns; repeat: true">
        </div>
    </div>
    <div>
        <div class="uk-overflow-hidden">
            <img src="images/dark.jpg" alt="Example image" class="uk-animation-reverse uk-transform-origin-top-right" uk-scrollspy="cls: uk-animation-kenburns; repeat: true">
        </div>
    </div>
</div>
