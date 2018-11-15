
Utility
A collection of useful utility classes to style your content.

Panel
UIkit uses panels to outline certain sections of your content. These can be arranged in grid columns from the Grid component component, for example.

Add the .uk-panel class to a <div> element to create a position context, set box-sizing to border-box, apply a clearfix and to remove the bottom margin of its last child element.

PREVIEW
MARKUP
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.


<div class="uk-child-width-1-3@s" uk-grid>
    <div>
        <div class="uk-panel">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</div>
    </div>
    <div>
        <div class="uk-panel">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</div>
    </div>
    <div>
        <div class="uk-panel">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</div>
    </div>
</div>


Scrollable panel
Add the .uk-panel-scrollable class to give the panel a fixed height and make it scrollable, if its content exceeds the height. You can also add one of the .uk-height-* classes to apply a different height.

PREVIEW
MARKUP
 Category 1
 Category 2
 Category 2.1
 Category 2.2
 Category 2.3
 Category 2.3.1
 Category 2.3.2
 Category 2.4
 Category 3
 Category 4

<div class="uk-panel uk-panel-scrollable">
    <ul class="uk-list">
        <li><label><input class="uk-checkbox" type="checkbox"> Category 1</label></li>
        <li>
            <label><input class="uk-checkbox" type="checkbox"> Category 2</label>
            <ul>
                <li><label><input class="uk-checkbox" type="checkbox"> Category 2.1</label></li>
                <li><label><input class="uk-checkbox" type="checkbox"> Category 2.2</label></li>
                <li>
                    <label><input class="uk-checkbox" type="checkbox"> Category 2.3</label>
                    <ul>
                        <li><label><input class="uk-checkbox" type="checkbox"> Category 2.3.1</label></li>
                        <li><label><input class="uk-checkbox" type="checkbox"> Category 2.3.2</label></li>
                    </ul>
                </li>
                <li><label><input class="uk-checkbox" type="checkbox"> Category 2.4</label></li>
            </ul>
        </li>
        <li><label><input class="uk-checkbox" type="checkbox"> Category 3</label></li>
        <li><label><input class="uk-checkbox" type="checkbox"> Category 4</label></li>
    </ul>

</div>


Clearing and floating
Floating elements are taken from the document flow and aligned to the left or right side of their container. It is important to clear floats or in the worst case, you might end up with a scrambled site. The following classes will help you to set up basic layouts.

CLASS	DESCRIPTION
.uk-float-left	Add this class to float the element to the left.
.uk-float-right	Add this class to float the element to the right.
.uk-clearfix	Add this class to a parent container to clear floats. Alternatively, you can create a new block format context, e.g. by adding the .uk-overflow-hidden class.
PREVIEW
MARKUP
Right
Left

<div class="uk-clearfix">
    <div class="uk-float-right">
        <div class="uk-card uk-card-default uk-card-body">Right</div>
    </div>
    <div class="uk-float-left">
        <div class="uk-card uk-card-default uk-card-body">Left</div>
    </div>
</div>


Overflow
These utilities provide different classes to modify an element's overflow behavior.

CLASS	DESCRIPTION
.uk-overflow-hidden	Add this class to clip content that exceeds the dimensions of its container.
.uk-overflow-auto	Add this class to create a container that provides a horizontal or vertical scrollbar whenever the elements content it are wider or higher than the container itself.
NOTE The .uk-overflow-auto class is useful when having to handle tables on a responsive website, which at some point would just get too big. It also works great on <pre> elements.

PREVIEW
MARKUP
TABLE HEADING	TABLE HEADING	TABLE HEADING	TABLE HEADING	TABLE HEADING	TABLE HEADING	TABLE HEADING	TABLE HEADING
Table Footer	Table Footer	Table Footer	Table Footer	Table Footer	Table Footer	Table Footer	Table Footer
Table Data	Table Data	Table Data	Table Data	Table Data	Table Data	Table Data	Table Data
Table Data	Table Data	Table Data	Table Data	Table Data	Table Data	Table Data	Table Data


<div class="uk-overflow-auto uk-height-small">
    <table class="uk-table uk-table-striped uk-table-condensed uk-text-nowrap">
        <thead>
            <tr>
                <th>Table Heading</th>
                <th>Table Heading</th>
                <th>Table Heading</th>
                <th>Table Heading</th>
                <th>Table Heading</th>
                <th>Table Heading</th>
                <th>Table Heading</th>
                <th>Table Heading</th>
            </tr>
        </thead>
        <tfoot>
            <tr>
                <td>Table Footer</td>
                <td>Table Footer</td>
                <td>Table Footer</td>
                <td>Table Footer</td>
                <td>Table Footer</td>
                <td>Table Footer</td>
                <td>Table Footer</td>
                <td>Table Footer</td>
            </tr>
        </tfoot>
        <tbody>
            <tr>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
            </tr>
            <tr>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
                <td>Table Data</td>
            </tr>
        </tbody>
    </table>
</div>



Overflow Auto
Add the uk-overflow-auto attribute to expand an element's height to make it fill the remaining height of a parent container. It provides a vertical scrollbar if its content is higher than the expanded height.

PREVIEW
MARKUP
Some content before the overflow auto container.


<div class="uk-height-medium">
    <div class="js-wrapper">

        <p>Some content before the overflow auto container.</p>

        <div uk-overflow-auto="selContainer: .uk-height-medium; selContent: .js-wrapper">
            <div class="uk-grid-small" uk-grid>
                <div class="uk-width-1-2"><img src="images/light.jpg" alt=""></div>
                <div class="uk-width-1-2"><img src="images/dark.jpg" alt=""></div>
                <div class="uk-width-1-2"><img src="images/photo.jpg" alt=""></div>
                <div class="uk-width-1-2"><img src="images/photo2.jpg" alt=""></div>
            </div>
        </div>

        <p>Some content after the overflow auto container.</p>

    </div>
</div>




Some content after the overflow auto container.

It's often used within the Modal component.

<div id="my-id" uk-modal>
    <div class="uk-modal-dialog" uk-overflow-auto></div>
</div>
PREVIEW
MARKUP
OPEN
You can change the target heights by adding the selContainer and selContent options to the attribute. Learn more


<a class="uk-button uk-button-default" href="#modal-overflow" uk-toggle>Open</a>

<div id="modal-overflow" uk-modal>
    <div class="uk-modal-dialog">

        <button class="uk-modal-close-default" type="button" uk-close></button>

        <div class="uk-modal-header">
            <h2 class="uk-modal-title">Headline</h2>
        </div>

        <div class="uk-modal-body" uk-overflow-auto>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>

        </div>

        <div class="uk-modal-footer uk-text-right">
            <button class="uk-button uk-button-default uk-modal-close" type="button">Cancel</button>
            <button class="uk-button uk-button-primary" type="button">Save</button>
        </div>

    </div>
</div>



OPTION	VALUE	DEFAULT	DESCRIPTION
selContainer	String	.uk-modal	CSS selector for the container element which provides the height.
selContent	String	.uk-modal-dialog	CSS selector for the element which wraps the inner content to provide its height.
Resize
These utilities provide different classes for resizing elements.

CLASS	DESCRIPTION
.uk-resize	Add this class to enable horizontal and vertical resizing.
.uk-resize-vertical	Add this class to enable only vertical resizing.
Grab and drag the bottom right corner of each box below to resize it

PREVIEW
MARKUP
            

<!-- Resize vertically -->
<div uk-grid>
    <div class="uk-width-1-2">...</div>
    <div class="uk-width-1-2">...</div>
</div>

<div class="uk-child-width-1-2" uk-grid>
    <div></div>
    <div></div>
</div>
            

        
            

<!-- Resize horizontally and vertically -->
<div uk-grid>
    <div class="uk-width-1-2">...</div>
    <div class="uk-width-1-2">...</div>
</div>

<div class="uk-child-width-1-2" uk-grid>
    <div></div>
    <div></div>
</div>
            

<div class="uk-child-width-1-2@s" uk-grid>
    <div>
        <pre class="uk-resize-vertical">
            <code>
&lt;!-- Resize vertically --&gt;
&lt;div uk-grid&gt;
    &lt;div class="uk-width-1-2"&gt;...&lt;/div&gt;
    &lt;div class="uk-width-1-2"&gt;...&lt;/div&gt;
&lt;/div&gt;

&lt;div class="uk-child-width-1-2" uk-grid&gt;
    &lt;div&gt;&lt;/div&gt;
    &lt;div&gt;&lt;/div&gt;
&lt;/div&gt;
            </code>
        </pre>
    </div>
    <div>
        <pre class="uk-resize">
            <code>
&lt;!-- Resize horizontally and vertically --&gt;
&lt;div uk-grid&gt;
    &lt;div class="uk-width-1-2"&gt;...&lt;/div&gt;
    &lt;div class="uk-width-1-2"&gt;...&lt;/div&gt;
&lt;/div&gt;

&lt;div class="uk-child-width-1-2" uk-grid&gt;
    &lt;div&gt;&lt;/div&gt;
    &lt;div&gt;&lt;/div&gt;
&lt;/div&gt;
            </code>
        </pre>
    </div>
</div>


        
Display
Add one of these classes to change the display properties of an element.

CLASS	DESCRIPTION
.uk-display-block	Forces the element to behave like a block element.
.uk-display-inline	Forces the element to behave like an inline element.
.uk-display-inline-block	Forces the element to behave like an inline-block element.
Inline
These classes are often used to create a position context on containers with an image as a child. The container keeps the same size as the image as well as the responsive behavior. That way content that is placed on top of the image with the Position component will not flow out of the image dimensions.

CLASS	DESCRIPTION
.uk-inline	Add this class to apply inline-block behavior to an element, add a max-width of 100% and to create a position context.
.uk-inline-clip	Same as .uk-inline, it but also clips overflowing child elements.
<div class="uk-inline">
    <img alt="">
    <div class="uk-position-cover"></div>
</div>
PREVIEW
MARKUP
Overlay



<div class="uk-inline">
    <img src="images/photo.jpg" width="300" alt="">
    <div class="uk-position-medium uk-position-cover uk-overlay uk-overlay-default uk-flex uk-flex-center uk-flex-middle">Overlay</div>
</div>




Responsive objects
In UIkit <img>, <canvas>, <audio> and <video> elements adapt to the width of their parent container by default. To apply responsive behavior to iframes, add the uk-responsive attribute . For other elements or to apply a different behavior, just add one of the following classes.

CLASS	DESCRIPTION
.uk-responsive-width	Add this class to apply the same responsive behavior to any other element. It adjusts the object's width according to its parent's width, keeping the original aspect ratio.
.uk-responsive-height	Add this class to adjust the object's height (instead of its width) according to its parent's height, keeping the original aspect ratio.
.uk-preserve-width	Add this class to avoid the default responsive behavior and preserve the original image dimensions. You can also add the class to a parent element and it will be applied to all relevant elements content it. If you are embedding Google Maps into your site, you may need this to fix the map's images.
<img class="uk-responsive-height" src="" alt="">

<iframe src="" width="" height="" frameborder="0" uk-responsive></iframe>
Border radius
To modify the border radius of an element, like an image, add one of the following classes.

CLASS	DESCRIPTION
.uk-border-rounded	Add this class to apply rounded corners.
.uk-border-circle	Add this class to apply a circled shape.
.uk-border-pill	Add this class to apply a pill shape.
PREVIEW
MARKUP
Border rounded Border circle Border pill
Box shadow
You can apply different box shadows to elements. Just add one of the following classes.

CLASS	DESCRIPTION
.uk-box-shadow-small	Add this class to apply a small box shadow.
.uk-box-shadow-medium	Add this class to apply a medium box shadow.
.uk-box-shadow-large	Add this class to apply a large box shadow.
.uk-box-shadow-xlarge	Add this class to apply a very large box shadow.
<div class="uk-box-shadow-small"></div>
PREVIEW
MARKUP
Small
Medium
Large
XLarge
Box shadow bottom
To apply a box shadow at the bottom of an element so that appears to be hovering, add the .uk-box-shadow-bottom class. This can also be combined with one of the other .uk-box-shadow-* modifiers.

<div class="uk-box-shadow-bottom"></div>
PREVIEW
MARKUP
Box shadow bottom
Hover
To apply a box shadow on hover, add one of the following classes. This can also be used to modify the shadow size on hover. To do so, just combine them with one of the classes above.

CLASS	DESCRIPTION
.uk-box-shadow-hover-small	Add this class to apply a small box shadow on hover.
.uk-box-shadow-hover-medium	Add this class to apply a medium box shadow on hover.
.uk-box-shadow-hover-large	Add this class to apply a large box shadow on hover.
.uk-box-shadow-hover-xlarge	Add this class to apply a very large box shadow on hover.
<div class="uk-box-shadow-hover-small"></div>
PREVIEW
MARKUP
Hover Small
Hover XLarge
Small + Hover Large
XLarge + Hover Medium
Drop cap
With the .uk-dropcap class you can achieve a drop cap within a text by adding it directly to the <p> element.

PREVIEW
MARKUP
Dorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

Logo
With the new .uk-logo class you can easily define your logo, for example within your navbar.

<a class="uk-logo" href=""></a>
PREVIEW
MARKUP
Logo
Add the .uk-light class from the Inverse component when displaying the image on dark backgrounds, so that its color will automatically be inverted for better visibility.

PREVIEW
MARKUP
Logo
Logo image
You can also use an <img> element, for example an SVG, as a logo.

<a class="uk-logo" href="">
    <img src="" alt="">
</a>
You can even automatically display alternative logos for light and dark backgrounds by using the Inverse component. Just add the .uk-logo-inverse class to a second logo image. Depending on the color mode, the inverted logo will be displayed when the .uk-light or .uk-dark class is applied to the parent element.

<div class="uk-light">
    <a class="uk-logo" href="">
        <img src="" alt="">
        <img class="uk-logo-inverse" src="" alt="">
    </a>
</div>
PREVIEW
MARKUP
 
 
NOTE To inject a SVG logo as inline SVG, use the SVG component.

Blend modes
Add one of the following classes to apply different blend modes to your backgrounds, for example when placing them on images. You can combine these with the Overlay component. For a better understanding of how background blend modes work, take a look at this CSS Tricks article.

CLASS	DESCRIPTION
.uk-blend-multiply	This class sets the blend mode to multiply.
.uk-blend-screen	This class sets the blend mode to screen.
.uk-blend-overlay	This class sets the blend mode to overlay.
.uk-blend-darken	This class sets the blend mode to darken.
.uk-blend-lighten	This class sets the blend mode to lighten.
.uk-blend-color-dodge	This class sets the blend mode to color dodge.
.uk-blend-color-burn	This class sets the blend mode to color burn.
.uk-blend-hard-light	This class sets the blend mode to hard light.
.uk-blend-soft-light	This class sets the blend mode to soft light.
.uk-blend-difference	This class sets the blend mode to difference.
.uk-blend-exclusion	This class sets the blend mode to exclusion.
.uk-blend-hue	This class sets the blend mode to hue.
.uk-blend-saturation	This class sets the blend mode to saturation.
.uk-blend-color	This class sets the blend mode to color.
.uk-blend-luminosity	This class sets the blend mode to luminosity.
<div class="uk-position-relative">
    <div class="uk-blend-multiply uk-overlay uk-overlay-primary"></div>
    <img src="" alt="">
</div>
PREVIEW
MARKUP
Blend Multiply
Multiply

 Blend Screen
Screen

 Blend Overlay
Overlay

 Blend Darken
Darken

 Blend Lighten
Lighten

 Blend Color Dodge
Color Dodge

 Blend Color Burn
Color Burn

 Blend Hard Light
Hard Light

 Blend Soft Light
Soft Light

 Blend Difference
Difference

 Blend Exclusion
Exclusion

 Blend Hue
Hue

 Blend Saturation
Saturation

 Blend Color
Color

 Blend Luminosity
Luminosity

Transform center
To center an element to itself, add the uk-transform-center class. This is particularly useful for absolute positioning.

PREVIEW
MARKUP

Transform origin
To modify the origin of an animation, like scaling, add one of the uk-transform-origin-* classes. This can be combined with the Animation component.

CLASS	DESCRIPTION
.uk-transform-origin-top-left	The transition originates from the top left.
.uk-transform-origin-top-center	The transition originates from the top.
.uk-transform-origin-top-right	The transition originates from the top right.
.uk-transform-origin-center-left	The transition originates from the left.
.uk-transform-origin-center-right	The transition originates from the right.
.uk-transform-origin-bottom-left	The transition originates from the bottom left.
.uk-transform-origin-bottom-center	The transition originates from the bottom.
.uk-transform-origin-bottom-right	The transition originates from the bottom right.
<div class="uk-transform-origin-bottom-right uk-animation-scale-up"></div>
PREVIEW
MARKUP
Bottom Right

Top Center

Bottom Center

Disabled
To disable the click behavior of any element, like a <a>, <button> or <iframe> element, add the .uk-disabled class.

PREVIEW
MARKUP
DISABLED
Drag
To apply a move cursor to elements that are being dragged, add the .uk-drag class.

<div class="uk-drag"></div>
PREVIEW
MARKUP
To create a box shadow on an upload area when dragging a file over it, add the .uk-dragover class.
