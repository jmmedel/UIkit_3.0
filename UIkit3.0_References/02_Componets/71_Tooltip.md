
Tooltip
Easily create a nice looking tooltip.

Usage
To apply this component, add the uk-tooltip attribute to an element. You also need to add the title: TEXT option to the attribute, whose value will represent your tooltip's text.

<div uk-tooltip="title: Hello World"></div>
If title is the only option in the attribute value, you can also use uk-tooltip="TEXT"

<div uk-tooltip="Hello World"></div>
PREVIEW
MARKUP
HOVER
Alignment
Add one of the following options to the uk-tooltip attribute to adjust the tooltip's alignment.

<button uk-tooltip="title: Hello World; pos: top-left"></button>
ATTRIBUTE	DESCRIPTION
pos: top	Aligns the tooltip to the top.
pos: top-left	Aligns the tooltip to the top left.
pos: top-right	Aligns the tooltip to the top right.
pos: bottom	Aligns the tooltip to the bottom.
pos: bottom-left	Aligns the tooltip to the bottom left.
pos: bottom-right	Aligns the tooltip to the bottom right.
pos: left	Aligns the tooltip to the left.
pos: right	Aligns the tooltip to the right.
PREVIEW
MARKUP
TOP  TOP LEFT  TOP RIGHT BOTTOM  BOTTOM LEFT BOTTOM RIGHT  LEFT  RIGHT

Delay
If you want the tooltip to appear with a little delay, just add the delay option to the uk-tooltip attribute with your value in milliseconds.

<div uk-tooltip="title: Hello World; delay: 500"></div>
PREVIEW
MARKUP
HOVER
Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
title	String	``	Tooltip text.
pos	String	top	Tooltip position.
offset	Number	false	Tooltip offset.
animation	String	uk-animation-scale-up	The space separated names of animations to use. Comma separate for animation out.
duration	Number	100	The animation duration.
delay	Number	0	The show delay.
cls	String	uk-active	The active class.
title is the Primary option and its key may be omitted, if it's the only option in the attribute value.

<span uk-tooltip="Hello World"></span>
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.tooltip(element, options);
Events
The following events will be triggered on elements, which are injected by this component:

NAME	DESCRIPTION
beforeshow	Fires before an item is shown. Can prevent showing by returning false.
show	Fires after an item is shown.
shown	Fires after the item's show animation has completed.
beforehide	Fires before an item is hidden. Can prevent hiding by returning false.
hide	Fires after an item's hide animation has started.
hidden	Fires after an item is hidden.
Example
UIkit.util.on(document, 'show', '.uk-tooltip.uk-active', function() {
  // do something
});
Methods
The following methods are available for the component:

Show
UIkit.tooltip(element).show();
Shows the Tooltip.

Hide
UIkit.tooltip(element).hide();
Hides the Tooltip.
