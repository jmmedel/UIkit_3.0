


Background
A collection of utility classes to add different backgrounds to elements.

Usage
To apply a background color to an element, add one of the following classes. The actual color for each modifier is defined by the UIkit style that you have chosen or customized.

CLASS	DESCRIPTION
.uk-background-default	Applies the default background color.
.uk-background-muted	Applies a muted background color.
.uk-background-primary	Applies the primary background color.
.uk-background-secondary	Applies a secondary background color.
<div class="uk-background-primary"></div>
NOTE To adapt your content for better visibility on each background, add the .uk-light or .uk-dark class from the Inverse component. Use the Padding component to add some padding to the elements.

PREVIEW
MARKUP
Default

Muted

Primary

Secondary

Size modifiers
This component features classes to specify the size of background images by keeping its intrinsic ratio.

CLASS	DESCRIPTION
.uk-background-cover	Scales the background image to completely cover the containing area.
.uk-background-contain	Scales the background image as far as its width and height can fit inside the containing area.
NOTE When using these classes, the background position automatically shifts to the middle and background-repeat is set to no-repeat.

<div class="uk-background-cover"></div>
PREVIEW
MARKUP
Cover

Contain

Position modifiers
To alter the background position of your image — which is in the top left hand corner of the area by default, add one of the following classes.

CLASS	DESCRIPTION
.uk-background-top-left	The initial position of the image is in the top left hand corner.
.uk-background-top-center	The initial position of the image is at the top.
.uk-background-top-right	The initial position of the image is in the top right hand corner.
.uk-background-center-left	The initial position of the image is on the left.
.uk-background-center-center	The initial position of the image is in the middle.
.uk-background-center-right	The initial position of the image is on the right.
.uk-background-bottom-left	The initial position of the image is in the bottom left hand corner.
.uk-background-bottom-center	The initial position of the image is at the bottom.
.uk-background-bottom-right	The initial position of the image is in the bottom right hand corner.
<div class="uk-background-top-left"></div>
PREVIEW
MARKUP
Top Right

Top Left

No repeat
To keep smaller images from repeating to fill the background area, add the .uk-background-norepeat class.

<div class="uk-background-norepeat"></div>
Attachment
You can also apply a fixed background attachment, so that the image remains in its position while scrolling the site.

<div class="uk-background-fixed"></div>
PREVIEW
MARKUP
Responsive
Add one of the following classes to limit the display of background images to certain viewport sizes. This is great in cases where the image and content overlap on a phone screen in a way that would make text illegible.

CLASS	DESCRIPTION
.uk-background-image@s	Displays the background image on device widths of 640px and larger.
.uk-background-image@m	Displays the background image on device widths of 960px and larger.
.uk-background-image@l	Displays the background image on device widths of 1200px and larger.
.uk-background-image@xl	Displays the background image on device widths of 1600px and larger.
<div class="uk-background-image@m"></div>
Resize your browser window to see the effect in the example below.

PREVIEW
MARKUP
Image not shown

Blend modes
Add one of the following classes to apply different blend modes to your background image. You can combine these with the background color classes, as well. For a better understanding of how background blend modes work, take a look at this CSS Tricks article.

CLASS	DESCRIPTION
.uk-background-blend-multiply	This class sets the blend mode to multiply.
.uk-background-blend-screen	This class sets the blend mode to screen.
.uk-background-blend-overlay	This class sets the blend mode to overlay.
.uk-background-blend-darken	This class sets the blend mode to darken.
.uk-background-blend-lighten	This class sets the blend mode to lighten.
.uk-background-blend-color-dodge	This class sets the blend mode to color dodge.
.uk-background-blend-color-burn	This class sets the blend mode to color burn.
.uk-background-blend-hard-light	This class sets the blend mode to hard light.
.uk-background-blend-soft-light	This class sets the blend mode to soft light.
.uk-background-blend-difference	This class sets the blend mode to difference.
.uk-background-blend-exclusion	This class sets the blend mode to exclusion.
.uk-background-blend-hue	This class sets the blend mode to hue.
.uk-background-blend-saturation	This class sets the blend mode to saturation.
.uk-background-blend-color	This class sets the blend mode to color.
.uk-background-blend-luminosity	This class sets the blend mode to luminosity.
<div class="uk-background-blend-multiply uk-background-primary"></div>
PREVIEW
MARKUP
Multiply

Screen

Overlay

Darken

Lighten

Color Dodge

Color Burn

Hard Light

Soft Light

Difference

Exclusion

Hue

Saturation

Color

Luminosity
