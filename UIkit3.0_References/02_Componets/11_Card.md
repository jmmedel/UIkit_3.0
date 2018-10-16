Card
Create layout boxes with different styles.

Usage
The Card component consists of the card itself, the card body and an optional card title. Typically, cards are arranged in grid columns from the Grid component.

CLASS	DESCRIPTION
.uk-card	Add this class to a <div> element to define the Card component.
.uk-card-body	Add this class to the card to create padding between the card and its content.
.uk-card-title	Add this class to a heading to define a card title.
<div class="uk-card uk-card-body">
    <h3 class="uk-card-title"></h3>
</div>
By default, a card is blank. That is why it is important to add a modifier class for styling. In our example we are using the .uk-card-default class.

PREVIEW
MARKUP
Default
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

<div class="uk-card uk-card-default uk-card-body uk-width-1-2@m">
    <h3 class="uk-card-title">Default</h3>
    <p>Lorem ipsum <a href="#">dolor</a> sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
</div>


Style modifiers
UIkit includes a number of modifiers that can be used to add a specific style to cards.

CLASS	DESCRIPTION
.uk-card-default	Add this class to create a visually styled box.
.uk-card-primary	Add this class to modify the card and emphasize it with a primary color.
.uk-card-secondary	Add this class to modify the card and give it a secondary background color.
<div class="uk-card uk-card-default"></div>

<div class="uk-card uk-card-primary"></div>

<div class="uk-card uk-card-secondary"></div>
PREVIEW
MARKUP
Default
Lorem ipsum dolor sit amet, consectetur adipisicing elit.

Primary
Lorem ipsum dolor sit amet, consectetur adipisicing elit.

Secondary
Lorem ipsum dolor sit amet, consectetur adipisicing elit.


<div class="uk-child-width-1-3@m uk-grid-small uk-grid-match" uk-grid>
    <div>
        <div class="uk-card uk-card-default uk-card-body">
            <h3 class="uk-card-title">Default</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
    </div>
    <div>
        <div class="uk-card uk-card-primary uk-card-body">
            <h3 class="uk-card-title">Primary</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
    </div>
    <div>
        <div class="uk-card uk-card-secondary uk-card-body">
            <h3 class="uk-card-title">Secondary</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
    </div>
</div>


Hover modifier
To create a hover effect on the card, add the .uk-card-hover class. This comes in handy when working with anchors and can be combined with the other card modifiers.

<div class="uk-card uk-card-hover"></div>
PREVIEW
MARKUP
Hover
Lorem ipsum dolor sit amet, consectetur adipisicing elit.

Default
Lorem ipsum dolor sit amet, consectetur adipisicing elit.

Primary
Lorem ipsum dolor sit amet, consectetur adipisicing elit.

Secondary
Lorem ipsum dolor sit amet, consectetur adipisicing elit.

Size modifiers
You can apply different size modifiers to cards that will decrease or increase their padding.

CLASS	DESCRIPTION
.uk-card-small	Add this class to apply a smaller padding.
.uk-card-large	Add this class to apply a larger padding.
<div class="uk-card uk-card-small uk-card-default"></div>

<div class="uk-card uk-card-large uk-card-default"></div>
PREVIEW
MARKUP
Small
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

Large
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

Header & footer
You can also divide a card into header and footer — around the default body. Just add the .uk-card-header or .uk-card-footer class to a <div> element inside the card.

<div class="uk-card">
    <div class="uk-card-header">
        <h3 class="uk-card-title"></h3>
    </div>
    <div class="uk-card-body"></div>
    <div class="uk-card-footer"></div>
</div>
PREVIEW
MARKUP

Title
April 01, 2016

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.

READ MORE
Media
To display an image inside a card without any spacing, add one of the following classes to a <div> around the <img> element. Mind that you need to modify the source order accordingly.

CLASS	DESCRIPTION
.uk-card-media-top	This class indicates that the media element is aligned to the top.
.uk-card-media-bottom	This class indicates that the media element is aligned to the bottom.
.uk-card-media-left	This class indicates that the media element is aligned to the left.
.uk-card-media-right	This class indicates that the media element is aligned to the right.
<div class="uk-card uk-card-default">
    <div class="uk-card-media-top">
        <img src="" alt="">
    </div>
    <div class="uk-card-body"></div>
</div>
PREVIEW
MARKUP

Media Top
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.

Media Bottom
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.


Horizontal alignment
The .uk-card-media-left or the .uk-card-media-right classes are used to reset border radius or similar where necessary. They don't create the actual layout.

To do that, you could for example add the .uk-cover-container class from the Cover component. Add the uk-cover attribute to the image element and use the Grid and Width components to achieve the alignment. Create a <canvas> element with your image's width and height, so that it will retain its dimensions, if the grid stacks on smaller viewports. This is just one way of creating a side by side layout.

<div class="uk-card uk-card-default uk-child-width-1-2" uk-grid>
    <div class="uk-card-media-left uk-cover-container">
        <img src="" alt="" uk-cover>
        <canvas width="" height=""></canvas>
    </div>
    <div>
        <div class="uk-card-body"></div>
    </div>
</div>
PREVIEW
MARKUP

Media Left
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.


Media Right
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.

Badge
To position a badge inside a card, add the .uk-card-badge class to a container element. To style the badge, you can use one of the other components, for example the Label.

<div class="uk-card uk-card-body">
    <div class="uk-card-badge uk-label"></div>
</div>
PREVIEW
MARKUP
BADGE
Title
Lorem ipsum color sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
