
Leader
Create dot leaders for pricing menus or tables of contents.

A leader, also known as a dot leader or a tab leader, is a repeating pattern used to visually connect content across horizontal spaces. It is most commonly used for restaurant menus, between the meals and prices, and for tables of contents, between titles and page numbers.

Usage
To apply this component, add the uk-leader attribute to the element on the left. A line of characters, by default dots, will then fill the remaining space between the item and its adjacent element.

<div uk-leader></div>
PREVIEW
MARKUP
Lorem ipsum dolor sit amet
$20.90

<div class = "uk-grid-small" uk-grid>
        <div class= "uk-width-expand" uk-leader > lorem ipsun dolor sit amet 
        </div>
        <div>$20.0m </div>
</div>



Fill character
To change the dot to any custom character, just add the fill: STRING option to the attribute.

<div uk-leader="fill: -"></div>
PREVIEW
MARKUP
Lorem ipsum dolor sit amet
$20.90
NOTE The default fill character can be set through CSS or a LESS variable.


<div class="uk-grid-small" uk-grid>
    <div class="uk-width-expand" uk-leader="fill: -">Lorem ipsum dolor sit amet</div>
    <div>$20.90</div>
</div>


.uk-leader-fill-content::before { content: '.'; }
:root { --uk-leader-fill-content: '.'; }
@leader-fill-content: '.';
Responsive
It's possible to disable the leader for different device widths by applying the media option to the attribute and adding the appropriate viewport width. Add a number in pixels, for example media: 640, or a breakpoint, for example media: @m. The leader will be shown from the specified viewport width and upwards, but not below.

<div uk-leader="media: @m"></div>
Component options
The table below lists the available settings of the uk-leader attribute. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
fill	String	``	Optional fill character.
media	Integer, String	false	Condition for the space filling - a width as integer (e.g. 640) or a breakpoint (e.g. @s, @m, @l, @xl) or any valid media query (e.g. (min-width: 900px)).
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.leader(element, options);
