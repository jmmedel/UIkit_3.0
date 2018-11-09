

SVG
Inject inline SVG images into the page markup and style them with CSS.

SVGs or Scalable Vector Graphics are really handy, for example to display a logo that remains crisp when scaling or that is animated. The SVG component provides more control to style and animate the image and its vector parts. It injects the image into the markup as an inline SVG including all attributes, like IDs, classes, width and height, so that they can easily be targeted using CSS.

Usage
To apply this component, add the uk-svg attribute to an <img> element.

<img src="" uk-svg>
Using the uk-svg attribute also allows you to inject a symbol from the SVG file. Just append the symbol's ID to the image path as you would in any fragmented URL.

PREVIEW
MARKUP
 
NOTE SVGs will adapt the current color for their stroke and fill color. To prevent this behavior, you can add the .uk-preserve class to the SVG itself or to elements inside the SVG.

Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
src	String	''	The SVG source URL. If a location hash is present, only the <symbol> of the SVG with the given ID is shown.
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.svg(element, options);
Properties
svg
A JavaScript Promise that will resolve with the added SVG Node.

UIkit.svg(element).svg.then(function(svg) { svg.querySelector('path').style.stroke = 'red';
