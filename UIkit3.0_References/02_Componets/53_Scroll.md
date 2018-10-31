


Scroll
Scroll smoothly when jumping to different sections on a page.

Usage
Simply add the uk-scroll attribute to any page-internal link that contains a URL fragment to add the smooth scrolling behavior.

<a href="#my-id" uk-scroll></a>
PREVIEW
MARKUP
SCROLL DOWN


<a class="uk-button uk-button-primary" href="#target" uk-scroll>Scroll down</a>


Callback after scroll
To receive a callback when scrolling has completed, you can listen to the scrolled event on the link element that triggered the scrolling.

<a id="js-scroll-trigger" href="#my-id" uk-scroll></a>
UIkit.util.on('#scroll-trigger', 'scrolled', function () {
    alert('Done.');
});
PREVIEW
MARKUP
DOWN WITH CALLBACK


<a id="js-scroll-trigger" class="uk-button uk-button-primary" href="#target" uk-scroll>Down with callback</a>

<script>
    UIkit.util.on('#js-scroll-trigger', 'scrolled', function () {
        alert('Done.');
    });
</script>



Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
duration	Number	1000	Animation duration in milliseconds.
offset	Number	0	Pixel offset added to scroll top.
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.scroll(element, options);
SCROLL UP

Events
The following events will be triggered on elements with this component attached:

NAME	DESCRIPTION
beforescroll	Fires before scroll begins. Can prevent scrolling by returning false.
scrolled	Fires after scrolling is finished.
Methods
The following methods are available for the component:

ScrollTo
UIkit.scroll(element).scrollTo(el);
Scroll to the given element.

NAME	TYPE	DEFAULT	DESCRIPTION
el	Node, Selector	undefined	The element to scroll to.
