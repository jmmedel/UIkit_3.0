

Image
Speed up page loading times and decrease traffic by only loading images as they enter the viewport.

The Image component improves page speed significantly by following these methods:

Only images which are initially in the viewport are loaded.
Other images are lazy loaded as they enter the viewport when scrolling.
An empty placeholder image is generated instantly to prevent content jumping while images are being loaded or not yet in the viewport.
Optionally, the placeholder image can have any kind of background or preload animation.
The Image components supports the img element and the CSS background-image property. The srcset attribute for images is supported as well creating the optimal images for different device widths and high resolution (retina) displays. The Image component even makes it possible to use srcset for the CSS background-image property.

Usage
To apply this component, add the uk-img attribute to an <img> element and add the data- prefix to the src attribute so that it reads data-src.

<img data-src="" width="" height="" alt="" uk-img>
The width and height attributes are required so an empty placeholder can be generated in the exact same size as the image. Alternatively, use data-width and data-height if you don't want to set the explicit attributes.

PREVIEW
MARKUP

Srcset
To use the srcset attribute, just prefix it as data-srcset.

<img data-src="" data-srcset="" sizes="" width="" height="" alt="" uk-img>
PREVIEW
MARKUP

Background image
To use this component with the CSS background-image property, add it to a <div> or any other element.

<div data-src="" uk-img>...</div>
PREVIEW
MARKUP
Background Image
Background image with Srcset
The Image component allows you to use srcset for background images. Just add the data-srcset attribute. If you need the sizes attribute, prefix it as data-sizes.

<div data-src="" data-srcset="" data-sizes="" uk-img>...</div>
PREVIEW
MARKUP
Background Image
Target
Usually, the image starts loading when it enters the viewport. To start loading images based on the viewport visibility of another element, use the target option. This is very useful to lazy load images in the Slideshow and Slider components.

<img data-src="" width="" height="" alt="" uk-img="target: .my-class">
The following example loads all images in the slides as soon as the slideshow enters the viewport. It uses !.uk-slideshow-items as a target selector. The ! looks up the DOM to find the next parent element with the .uk-slideshow-item class.

PREVIEW
MARKUP

Load previous and next
It's also possible to load only the image of the active slide and lazy load the images of the other slides. Just target the previous and next slides for each image by using the target: !* -*, !* +* option. There are two exceptions where you have to select the first and the last slides.

SELECTOR	DESCRIPTION
!* -*	Looks for the direct parent (!*) and selects the preceding element (-*).
!* +*	Looks for the direct parent (!*) and selects the succeeding element (+*).
!.uk-slideshow-items > :last-child	Looks for the next parent element with the .uk-slideshow-item class and selects the last child.
!.uk-slideshow-items > :first-child	Looks for the next parent element with the .uk-slideshow-item class and selects the first child.
<ul class="uk-slideshow-items">
    <li>
        <img data-src="" width="" height="" alt="" uk-img="target: !ul > :last-child, !* +*">
    </li>
    <li>
        <img data-src="" width="" height="" alt="" uk-img="target: !* -*, !* +*">
    </li>
    <li>
        <img data-src="" width="" height="" alt="" uk-img="target: !* -*, !* +*">
    </li>
    <li>
        <img data-src="" width="" height="" alt="" uk-img="target: !* -*, !ul > :first-child">
    </li>
</ul>
PREVIEW
MARKUP

Custom placeholder
By default, the placeholder image is transparent. Use the img[data-src][src*='data:image'] selector to add a custom background or preload animation.

img[data-src][src*='data:image'] { background: rgba(0,0,0,0.1); }
Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
dataSrc	String	''	The image's src attribute.
dataSrcset	String	false	The image's srcset attribute.
sizes	String	false	The image's sizes attribute.
width	String	false	The image's width attribute. It will be used to determine the placeholder's width and the position of the image in the document.
height	String	false	The image's height attribute. It will be used to determine the placeholder's height and the position of the image in the document.
offsetTop	String	'50vh'	The offset increases the viewport's bounding box vertically before computing an intersection with the image.
offsetLeft	String	0	The offset increases the viewport's bounding box horizontally before computing an intersection with the image.
target	String	false	A list of targets who's bounding boxes will be used to compute an intersection with the image. Defaults to the image itself.
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.img(element, options);



