

Parallax
Animate CSS properties depending on the scroll position of the document.

Usage
To apply this component, add the uk-parallax attribute to any element. Add an option with the desired animation target value for each CSS property you want to animate.

<div uk-parallax="bgy: -200">...</div>
PREVIEW
MARKUP
Headline
Animated properties
You can use explicit CSS property names (e.g. width or scale) and a number of shorthands and special properties (e.g. bgy for background-position-y).

OPTION	DESCRIPTION
x	Animate translateX in pixels or percent.
y	Animate translateY in pixels or percent.
bgy	Animate a background image (y-axis).
bgx	Animate a background image (x-axis).
rotate	Animate rotation clockwise in degree.
scale	Animate scaling.
color	Animate color (needs start and stop value).
background-color	Animate background-color (needs start and stop value).
border-color	Animate border color (needs start and stop value).
opacity	Animate the opacity.
blur	Animate the blur filter.
hue	Animate the hue rotation filter.
grayscale	Animate the grayscale filter.
invert	Animate the invert filter.
saturate	Animate the saturate filter.
sepia	Animate the sepia filter.
NOTE You can basically animate any CSS property that has a single value, like width and height, by adding it to the attribute.

Start and end values
Properties are always animated from their current value to the target value you set in the option. However, you can also define a start value yourself. This is done by passing two values separated by comma.

NOTE Properties that do not have a matching CSS property, like CSS filters and transforms, always require a start and a stop value.

<div uk-parallax="opacity: 0,1">...</div>
PREVIEW
MARKUP
Headline
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

Multiple steps
You can define multiple steps for a property by using a comma separated list of values.

<div uk-parallax="x: 0,50,150">...</div>
PREVIEW
MARKUP
Headline
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

Viewport position
Using the viewport option you can adjust the animation duration. The value defines how far inside the viewport the target element is scrolled until the animation is completed. With the value 1 or false, the animation lasts as long as the element is in the viewport (default behavior). Setting it to 0.5, for example, animates the property until the scroll position reaches the middle of the target element.

<div uk-parallax="viewport: 0.5">...</div>
PREVIEW
MARKUP
Headline
Nesting
Different parallax animations can easily be nested.

<div uk-parallax="bgx: -50">
    <div uk-parallax="x: -100, 100">...</div>
</div>
PREVIEW
MARKUP
Headline
Target
Usually, the animation lasts as long as the element itself is in the viewport. To start and stop the animation based on the viewport visibility of another element, use the target option. This can be helpful when using nested animations.

<div id="target">
    <div uk-parallax="target: #target">...</div>
</div>
PREVIEW
MARKUP
Headline
Easing
To adjust the easing of the animation, add the easing option. Lower values will cause a faster transition in the beginning, higher values will cause a faster transition in the end of the animation.

PREVIEW
MARKUP
0
0.5
0.6
0.8
1
2
4
Colors
You can also transition from one color to another, for example for borders, backgrounds or text colors. Define colors using rgb() definitions, color keywords or hex values.

<div uk-parallax="border-color: #00f,#f00">...</div>
PREVIEW
MARKUP
Headline
Filters
CSS filters are an easy way to add graphical effects to any element on your page. While they are still an experimental feature for some browsers, you can safely use them as long as your usability does not suffer. Using the Parallax component, you can dynamically change the amount of a filter on your element.

<div uk-parallax="blur: 10; sepia: 100;">...</div>
PREVIEW
MARKUP
Headline
Responsive
It's possible to disable the parallax for different device widths by applying the media option to the attribute and adding the appropriate viewport width. Add a number in pixel, for example media: 640, or a breakpoint, for example media: @m. The parallax will be shown from the specified viewport width and upwards, but not below.

<div uk-parallax="media: @m"></div>
Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
easing	Number	1	Animation easing during scrolling
target	String	false	Element dimension reference for animation duration.
viewport	Number	1	Animation range depending on the viewport.
media	Integer, String	false	Condition for the active status - a width as integer (e.g. 640) or a breakpoint (e.g. @s, @m, @l, @xl) or any valid media query (e.g. (min-width: 900px)).
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.parallax(element, options);
