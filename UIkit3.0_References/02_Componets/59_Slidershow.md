

Slideshow
Create a responsive slideshow with images and videos.

The Slideshow component is fully responsive and supports touch and swipe navigation as well as mouse drag for desktops. When swiping between slides, the animation literally sticks at your fingertips or mouse cursor. It even accelerates to keep up with your pace when you click through previous and next navigation. All animations are hardware accelerated for a smoother performance.

Usage
To apply this component, add the uk-slideshow attribute to a container element and create a list of slides with the .uk-slideshow-items class.

Add an image in the background of each slide using the uk-cover attribute from the Cover component.

<div uk-slideshow>
    <ul class="uk-slideshow-items">
        <li>
            <img src="" alt="" uk-cover>
        </li>
    </ul>
</div>
PREVIEW
MARKUP



<div class="uk-position-relative uk-visible-toggle uk-light" uk-slideshow>

    <ul class="uk-slideshow-items">
        <li>
            <img src="images/photo.jpg" alt="" uk-cover>
        </li>
        <li>
            <img src="images/dark.jpg" alt="" uk-cover>
        </li>
        <li>
            <img src="images/light.jpg" alt="" uk-cover>
        </li>
    </ul>

    <a class="uk-position-center-left uk-position-small uk-hidden-hover" href="#" uk-slidenav-previous uk-slideshow-item="previous"></a>
    <a class="uk-position-center-right uk-position-small uk-hidden-hover" href="#" uk-slidenav-next uk-slideshow-item="next"></a>

</div>


NOTE To lazy load images in the slides, take a look at the Image component.

Animations
By default, the slideshow uses a slide animation. You can set the animation option to use a different animation. Possible values are as follows:

ANIMATION	DESCRIPTION
slide	Slides slide in side by side.
fade	Slides fade in.
scale	Slides are scaled up and fade out.
pull	Slides are pulled from the deck.
push	Slides are pushed to the deck.
<div uk-slideshow="animation: fade">...</div>
PREVIEW
MARKUP
Slide

Fade

Scale

Pull

Push

Autoplay



<div class="uk-child-width-1-2@m" uk-grid>
    <div>

        <div class="uk-h3">Slide</div>

        <div class="uk-position-relative uk-visible-toggle uk-light" uk-slideshow>

            <ul class="uk-slideshow-items">
                <li>
                    <img src="images/photo.jpg" alt="" uk-cover>
                </li>
                <li>
                    <img src="images/dark.jpg" alt="" uk-cover>
                </li>
                <li>
                    <img src="images/light.jpg" alt="" uk-cover>
                </li>
            </ul>

            <a class="uk-position-center-left uk-position-small uk-hidden-hover" href="#" uk-slidenav-previous uk-slideshow-item="previous"></a>
            <a class="uk-position-center-right uk-position-small uk-hidden-hover" href="#" uk-slidenav-next uk-slideshow-item="next"></a>

        </div>

    </div>
    <div>

        <div class="uk-h3">Fade</div>

        <div class="uk-position-relative uk-visible-toggle uk-light" uk-slideshow="animation: fade">

            <ul class="uk-slideshow-items">
                <li>
                    <img src="images/photo.jpg" alt="" uk-cover>
                </li>
                <li>
                    <img src="images/dark.jpg" alt="" uk-cover>
                </li>
                <li>
                    <img src="images/light.jpg" alt="" uk-cover>
                </li>
            </ul>

            <a class="uk-position-center-left uk-position-small uk-hidden-hover" href="#" uk-slidenav-previous uk-slideshow-item="previous"></a>
            <a class="uk-position-center-right uk-position-small uk-hidden-hover" href="#" uk-slidenav-next uk-slideshow-item="next"></a>

        </div>

    </div>
    <div>

        <div class="uk-h3">Scale</div>

        <div class="uk-position-relative uk-visible-toggle uk-light" uk-slideshow="animation: scale">

            <ul class="uk-slideshow-items">
                <li>
                    <img src="images/photo.jpg" alt="" uk-cover>
                </li>
                <li>
                    <img src="images/dark.jpg" alt="" uk-cover>
                </li>
                <li>
                    <img src="images/light.jpg" alt="" uk-cover>
                </li>
            </ul>

            <a class="uk-position-center-left uk-position-small uk-hidden-hover" href="#" uk-slidenav-previous uk-slideshow-item="previous"></a>
            <a class="uk-position-center-right uk-position-small uk-hidden-hover" href="#" uk-slidenav-next uk-slideshow-item="next"></a>

        </div>

    </div>
    <div>

        <div class="uk-h3">Pull</div>

        <div class="uk-position-relative uk-visible-toggle uk-light" uk-slideshow="animation: pull">

            <ul class="uk-slideshow-items">
                <li>
                    <img src="images/photo.jpg" alt="" uk-cover>
                </li>
                <li>
                    <img src="images/dark.jpg" alt="" uk-cover>
                </li>
                <li>
                    <img src="images/light.jpg" alt="" uk-cover>
                </li>
            </ul>

            <a class="uk-position-center-left uk-position-small uk-hidden-hover" href="#" uk-slidenav-previous uk-slideshow-item="previous"></a>
            <a class="uk-position-center-right uk-position-small uk-hidden-hover" href="#" uk-slidenav-next uk-slideshow-item="next"></a>

        </div>

    </div>
    <div>

        <div class="uk-h3">Push</div>

        <div class="uk-position-relative uk-visible-toggle uk-light" uk-slideshow="animation: push">

            <ul class="uk-slideshow-items">
                <li>
                    <img src="images/photo.jpg" alt="" uk-cover>
                </li>
                <li>
                    <img src="images/dark.jpg" alt="" uk-cover>
                </li>
                <li>
                    <img src="images/light.jpg" alt="" uk-cover>
                </li>
            </ul>

            <a class="uk-position-center-left uk-position-small uk-hidden-hover" href="#" uk-slidenav-previous uk-slideshow-item="previous"></a>
            <a class="uk-position-center-right uk-position-small uk-hidden-hover" href="#" uk-slidenav-next uk-slideshow-item="next"></a>

        </div>

    </div>
</div>




To activate autoplay, just add the autoplay: true option to the attribute. You can also set the interval in milliseconds between switching slides using autoplay-interval: 6000. To pause autoplay when hovering the slideshow, use pause-on-hover: true.

<div uk-slideshow="autoplay: true">...</div>
Infinite Scrolling
By default, infinite scrolling is enabled. To disable this behavior, just add the finite: true option to the attribute.

<div uk-slideshow="finite: true">...</div>
Ratio
The slideshow always takes up the full width of its parent container. The height adapts according to the defined ratio. To change the default ratio of 16:9, just add the ratio option to the attribute. It's recommended to use the same ratio as the background images. For example, just use their width and height, like 1600:1200.

<div uk-slideshow="ratio: 7:3">...</div>
PREVIEW
MARKUP




<div class="uk-position-relative uk-visible-toggle uk-light" uk-slideshow="ratio: 7:3; animation: push">

    <ul class="uk-slideshow-items">
        <li>
            <img src="images/photo.jpg" alt="" uk-cover>
        </li>
        <li>
            <img src="images/dark.jpg" alt="" uk-cover>
        </li>
        <li>
            <img src="images/light.jpg" alt="" uk-cover>
        </li>
    </ul>

    <a class="uk-position-center-left uk-position-small uk-hidden-hover" href="#" uk-slidenav-previous uk-slideshow-item="previous"></a>
    <a class="uk-position-center-right uk-position-small uk-hidden-hover" href="#" uk-slidenav-next uk-slideshow-item="next"></a>

</div>




Min/Max height
By default, the slideshow height adopts to the defined ratio. A minimum or maximum height can be set using the min-height and max-height options.

<div uk-slideshow="min-height: 300; max-height: 600">...</div>
PREVIEW
MARKUP

Viewport height
Adding the uk-height-viewport attribute from the Height component to the list of slideshow items will stretch the height to fill the whole viewport. You can set the min-height option to define a minimum height.

<div uk-slideshow>
    <ul class="uk-slideshow-items" uk-height-viewport="min-height: 300">...</ul>
</div>
PREVIEW
MARKUP

NOTE This example is set to 70% of the viewport height.

Navigation
To navigate through your slides, just use the uk-slideshow-item attribute. To target the slides, set the attribute of every nav item to the index number of the respective slideshow item. The elements with the uk-slideshow-item attribute need to be inside the uk-slideshow container. Setting the attribute to next and previous will switch to the adjacent slides.

<div uk-slideshow>

    <ul class="uk-slideshow-items">...</ul>

    <a href="#" uk-slideshow-item="previous">...</a>
    <a href="#" uk-slideshow-item="next">...</a>

    <ul>
        <li uk-slideshow-item="0"><a href="#">...</a></li>
        <li uk-slideshow-item="1"><a href="#">...</a></li>
        <li uk-slideshow-item="2"><a href="#">...</a></li>
    </ul>

</div>
The flexibility of the Slideshow component allows you to use any of the other UIkit components to navigate through items. For example the Slidenav, Dotnav and Thumbnav components can be used to style the slideshow navigations.

If there is no item specific content in the navigation items, you can also add the .uk-slideshow-nav class instead of adding navigation items manually. It will generate its items automatically using <li><a href="#"></a></li> as markup. This is a useful shortcut when using the Dotnav.

<div uk-slideshow>

    <ul class="uk-slideshow-items">...</ul>

    <ul class="uk-slideshow-nav uk-dotnav"></ul>

</div>
PREVIEW
MARKUP

NOTE For better visibility of overlaying navigations, add the .uk-light or .uk-dark class from the Inverse component.

Videos
The slideshow is not restricted to images. Other media, like videos, can be positioned in the background of each slide using the uk-cover attribute from the Cover component. Videos are muted, and play automatically. The video will pause whenever it's not visible, and resume once it becomes visible again.

<div uk-slideshow>
    <ul class="uk-slideshow-items">
        <li>
            <video src="" autoplay loop muted playslinline uk-cover></video>
        </li>
        <li>
            <iframe src="" frameborder="0" uk-cover></iframe>
        </li>
    </ul>
</div>
PREVIEW
MARKUP

Ken Burns effect
To add a simple Ken Burns effect, wrap the image with a div and add the .uk-position-cover and .uk-animation-kenburns classes. You can also apply the .uk-animation-reverse or one of the .uk-transform-origin-* classes from the Utility component to modify the effect.

<div uk-slideshow>
    <ul class="uk-slideshow-items">
        <li>
            <div class="uk-position-cover uk-animation-kenburns uk-animation-reverse uk-transform-origin-center-left">
                <img src="" alt="" uk-cover>
            </div>
        </li>
    </ul>
</div>
PREVIEW
MARKUP

Content overlays
Add content overlays using the Position component. It allows you to place the content anywhere inside the slide.

<div uk-slideshow>
    <ul class="uk-slideshow-items">
        <li>
            <img src="" alt="" uk-cover>
            <div class="uk-position-center uk-position-small">

                <!-- The content goes here -->

            </div>
        </li>
    </ul>
</div>
NOTE To adapt your content for better visibility on each image, add the .uk-light or .uk-dark class from the Inverse component or use the Overlay to add any style to the overlay box.

PREVIEW
MARKUP

Center
Lorem ipsum dolor sit amet, consectetur adipiscing elit.

Content parallax
Add the uk-slideshow-parallax attribute to any element inside the slides to animate it together with the slideshow animation. Add an option with the desired animation values for each CSS property you want to animate. Define at least one start and end value. It can be done by passing two values separated by a comma.

This functionality is inherited from the Parallax component, and it allows to animate CSS properties depending on the scroll position of the slideshow animation. Take a look at the possible properties that can be animated.

<div uk-slideshow>
    <ul class="uk-slideshow-items">
        <li>
            <img src="" alt="" uk-cover>
            <div class="uk-position-center uk-position-small">

                <div uk-slideshow-parallax="x: 100,-100">

                    <!-- The content goes here -->

                </div>

            </div>
        </li>
    </ul>
</div>
In the example above, the content will start at 100 and animate half way to 0 while the slide moves in. When the slide starts again to move out, the content will continue to animate to -100. This works because the start and end values have the same distance. For different distances, three values are needed: Start (Slide animates in), Middle (Slide is centered), End (Slide animates out).

<div uk-slideshow-parallax="x: 300,0,-100">...</div>
The next example defines different in and out animations. The content slides in by moving from 100 to 0 and fades out from 1 to 0.

<div uk-slideshow-parallax="x: 100,0,0; opacity: 1,1,0">...</div>
PREVIEW
MARKUP

Heading
Lorem ipsum dolor sit amet.

Advanced effects
The parallax attribute can be used to add additional effects to the slideshow animations. In the following example the push animation is extended by dimming out and scaling down the image when it's sliding out.

<div uk-slideshow="animation: push">
    <ul class="uk-slideshow-items">
        <li>
            <div class="uk-position-cover" uk-slideshow-parallax="scale: 1.2,1.2,1">
                <img src="" alt="" uk-cover>
            </div>
            <div class="uk-position-cover" uk-slideshow-parallax="opacity: 0,0,0.2; backgroundColor: #000,#000"></div>
        </li>
    </ul>
</div>
PREVIEW
MARKUP

Heading
Lorem ipsum dolor sit amet.

Content transitions
Transition classes from the Transition component are triggered automatically inside slides. Contrary to the parallax effect, transitions are not attached to the slideshow animation and start playing independently after the slideshow animation.

<div uk-slideshow>
    <ul class="uk-slideshow-items">
        <li>
            <img src="" alt="" uk-cover>
            <div class="uk-position-bottom uk-position-small">

                <div class="uk-transition-slide-bottom">

                    <!-- The content goes here -->

                </div>

            </div>
        </li>
    </ul>
</div>
Together with the Overlay component, content transitions are used to build a classic caption for the slideshow.

PREVIEW
MARKUP

Bottom
Lorem ipsum dolor sit amet, consectetur adipiscing elit.

Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

Slideshow
OPTION	VALUE	DEFAULT	DESCRIPTION
animation	String	slide	Slideshow animation mode: slide, fade, scale, pull or push.
autoplay	Boolean	false	Slideshow autoplays.
autoplay-interval	Number	7000	The delay between switching slides in autoplay mode.
finite	Boolean	false	Disable infinite sliding.
pause-on-hover	Boolean	true	Pause autoplay mode on hover.
index	Number	0	Slideshow item to show. 0 based index.
velocity	Number	1	The animation velocity (pixel/ms).
ratio	Boolean, String	16:9	The ratio. (false prevents height adjustment)
min-height	Boolean, Number	false	The minimum height.
max-height	Boolean, Number	false	The maximum height.
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.slideshow(element, options);
Events
The following events will be triggered on elements with this component attached:

NAME	DESCRIPTION
beforeitemshow	Fires before an item is shown.
itemshow	Fires after an item is shown.
itemshown	Fires after an item's show animation has completed.
beforeitemhide	Fires before an item is hidden.
itemhide	Fires after an item's hide animation has started.
itemhidden	Fires after an item's hide animation has completed.
Methods
The following methods are available for the component:

Show
UIkit.slideshow(element).show(index);
Shows the slideshow item.

startAutoplay
UIkit.slideshow(element).startAutoplay();
Starts the slideshow autoplay.

stopAutoplay
UIkit.slideshow(element).stopAutoplay();
Stops the slideshow autoplay.
