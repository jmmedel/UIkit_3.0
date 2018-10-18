


Lightbox
Create a responsive lightbox gallery with images and videos.

The lightbox component is fully responsive and supports touch and swipe navigation, as well as mouse drag for desktops. When swiping between slides the animation literally sticks at your fingertip or mouse cursor. Clicking fast on the previous and next navigation, will make animations even accelerate to keep up with your pace. All animations are hardware accelerated for a smoother performance.

Usage
To apply this component, add the uk-lightbox attribute to a container to turn all anchors inside that container into lightbox links.

<div uk-lightbox>
    <a href="image.jpg"></a>
</div>
PREVIEW
MARKUP
OPEN LIGHTBOX
Alt Attribute
To add an alt attribute to the image in the lightbox, set the data-alt attribute on an anchor.

<div uk-lightbox>
    <a href="image.jpg" data-alt="Image"></a>
</div>
PREVIEW
MARKUP
OPEN LIGHTBOX
Caption
To display a caption at the bottom of the lightbox, set the data-caption attribute on an anchor.

<div uk-lightbox>
    <a href="image.jpg" data-caption="Caption"></a>
</div>
PREVIEW
MARKUP
OPEN LIGHTBOX
Animations
By default, the Lightbox gallery uses a slide animation. You can set the animation option to use a different one. Possible values are slide, fade and scale.

<div uk-lightbox="animation: fade">
    <a href="image.jpg"></a>
</div>
PREVIEW
MARKUP
Slide



Fade



Scale



Content sources
A lightbox is not restricted to images. Other media, like videos, can be displayed as well. The video will pause whenever it's not visible and resume once it becomes visible again. To display a poster image for a video, set the data-poster attribute.

<div uk-lightbox>
    <a class="uk-button" href="video.mp4" data-poster="image.jpg"></a>
    <a class="uk-button" href="https://www.youtube.com/watch?v=YE7VzlLtp-4"></a>
    <a class="uk-button" href="https://vimeo.com/1084537"></a>
    <a class="uk-button" href="https://www.google.com/maps"></a>
</div>
PREVIEW
MARKUP
IMAGE VIDEO YOUTUBE VIMEO GOOGLE MAPS
NOTE Use youtube-nocookie.com within the YouTube link and the lightbox will use the domain to embed the YouTube video.

Manual content type
The Lightbox uses the href attribute to figure out the type of the linked content. If no filename extension is defined in the path, just add the data-type attribute to the <a> tag.

Hint YouTube and Vimeo Urls will be handled automatically.

OPTION	DESCRIPTION
data-type="image"	The content type is an image.
data-type="video"	The content type is a video.
data-type="iframe"	The content type is a regular website.
Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

Lightbox
OPTION	VALUE	DEFAULT	DESCRIPTION
animation	String	slide	Lightbox animation mode: slide, fade or scale.
autoplay	Number	0	Lightbox autoplays. (Delay in milliseconds)
autoplay-interval	Number	0	The delay between switching slides in autoplay mode.
pause-on-hover	Boolean	false	Pause autoplay mode on hover.
video-autoplay	Boolean	false	Lightbox videos autoplay.
index	String, Integer	0	Lightbox item to show. 0 based index.
toggle	CSS selector	a	Toggle selector - opens the Lightbox Panel upon click.
JavaScript
Learn more about JavaScript components.

Initialization
// To apply lightbox to a group of links
UIkit.lightbox(element, options);

// To dynamically initialize the lightbox panel
UIkit.lightboxPanel(panelOptions);
Methods
The following methods are available for the component:

Show
UIkit.lightbox(element).show(index);
Shows the Lightbox's Panel and item.

Hide
UIkit.lightbox(element).hide();
Hides the Lightbox's Panel.

Lightbox Panel Options
If you only want to use the lightbox panel directly through the JS API, you can set the following options.

OPTION	VALUE	DEFAULT	DESCRIPTION
animation	String	slide	Lightbox animation mode: slide, fade or scale.
autoplay	Boolean	false	Lightbox autoplays.
autoplay-interval	Number	7000	The delay between switching slides in autoplay mode.
pause-on-hover	Boolean	false	Pause autoplay mode on hover.
video-autoplay	Boolean	false	Lightbox videos autoplay.
index	Number	0	The initial item to show. (zero based)
velocity	Number	2	The animation velocity (pixel/ms).
preload	Number	1	The number of items to preload. (left and right of the currently active item)
items	Array	[]	An array of items to display, e.g. [{source: 'images/size1.jpg', caption: '900x600'}]
template	String	Default markup	The template string.
delay-controls	Number	3000	Delay time before controls fade out in ms.
Events
The following events will be triggered on elements with this component attached:

NAME	DESCRIPTION
beforeshow	Fires before the Lightbox is shown.
beforehide	Fires before the Lightbox is hidden.
show	Fires after the Lightbox is shown.
shown	Fires after the Lightbox's show animation has completed.
hide	Fires after the Lightbox's hide animation has started.
hidden	Fires after the Lightbox is hidden.
itemload	Fires when an item loads.
beforeitemshow	Fires before an item is shown.
itemshow	Fires after an item is shown.
itemshown	Fires after an item's show animation has completed.
beforeitemhide	Fires before an item is hidden.
itemhide	Fires after an item's hide animation has started.
itemhidden	Fires after an item's hide animation has completed.
Methods
The following methods are available for the component:

Show
UIkit.lightboxPanel(element).show(index);
Shows the Lightbox Panel and item.

NAME	TYPE	DEFAULT	DESCRIPTION
index	String, Integer	0	Lightbox item to show. 0 based index.
Hide
UIkit.lightboxPanel(element).hide();
Hides the Lightbox Panel.

startAutoplay
UIkit.lightboxPanel(element).startAutoplay();
Starts the Lightbox's autoplay.

stopAutoplay
UIkit.lightboxPanel(element).stopAutoplay();
Stops the Lightbox's autoplay.


