

Base
This component provides the default style for all HTML elements.

Normalize.css
The Base component utilizes styling of the famous Normalize.css to render elements consistently across all browsers and applies its default styling like colors, margins, font-sizes and more.

NOTE Form, Button and Table elements are not normalized or styled by default. This happens in their specific component class. UIkit tries to apply as little styling as possible to plain HTML elements in order to remain robust and conflict free with 3rd party CSS.

Links
Turn text into hypertext using the <a> element. You can also add the .uk-link class to a <span> or similar element to apply the default link styling. For additional styling options, take a look at the Link component.

Text-level semantics
The following list gives you a short overview of the most commonly used text-level semantics and how to utilize them.

ELEMENT	DESCRIPTION
<abbr>	Define an abbreviation using the abbr element with a title.
<b>	Create bold text with the b element.
<cite>	Define the title of a work with the cite element.
<code>	Define inline code snippets using the code element.
<del>	Mark document changes as deleted text using the del element.
<dfn>	Create a definition term using the dfn element with a title.
<em>	Emphasize text using the em element.
<i>	Set off part of a text by using the i element.
<ins>	Mark document changes as inserted text using the ins element.
<kbd>	Use a keybord input element to display input in the browser's default monospace font.
<mark>	Highlight text with no semantic meaning using the mark element.
<q>	Define inline quotations using a q element inside a q element.
<s>	Define text with a strikethrough using the s element.
<samp>	Define sample output with a samp element.
<small>	De-emphasize text for small print using the small element.
<span>	Define an inline-container using the span element.
<strong>	Imply extra importance using the strong element.
<sub>	Define subscript text using the sub element..
<sup>	Define superscript text using the sup element.
<u>	Define underlined text using the u element.
<var>	Define a variable using the var element.
Embedded content
Images and other elements like <audio>, <canvas>, <img>, <svg> and <video> are responsive by default in UIkit. If the layout is narrowed, they adjust their size and keep their proportions. To prevent this behavior, add the .uk-preserve-width class from the Utility component to the element or any container.

Resize the browser window to see the responsive behavior of the image.

PREVIEW
MARKUP
Image

<div class="uk-width-large">
    <img src="images/photo.jpg" alt="Image">
</div>

Paragraphs
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>

Create a paragraph by using the <p> element.

PREVIEW
MARKUP
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

Headings

Use the <h1> to <h6> elements to define your headings.

Add the .uk-h1, .uk-h2, .uk-h3, .uk-h4, .uk-h5 or .uk-h6 class to alter the size of your headings, for example have a h1 look like a h3. For additional styling options, take a look at the Heading component.

PREVIEW
MARKUP
h1 Heading 1
h2 Heading 2
h3 Heading 3
h4 Heading 4
h5 Heading 5
h6 Heading 6

<h1>h1 Heading 1</h1>
<h2>h2 Heading 2</h2>
<h3>h3 Heading 3</h3>
<h4>h4 Heading 4</h4>
<h5>h5 Heading 5</h5>
<h6>h6 Heading 6</h6>

Lists
Create an unordered list using the <ul> element and the <ol> element for ordered lists. The <li> element defines the list item. For additional styling options, take a look at the List component.

PREVIEW
MARKUP
Item 1
Item 2
Item 1
Item 2
Item 1
Item 2
Item 3
Item 4

<ul>
    <li>Item 1</li>
    <li>Item 2
        <ul>
            <li>Item 1</li>
            <li>Item 2
                <ul>
                    <li>Item 1</li>
                    <li>Item 2</li>
                </ul>
            </li>
        </ul>
    </li>
    <li>Item 3</li>
    <li>Item 4</li>
</ul>


Description list
Create a description list using the <dl> element. Use <dt> to define the term and <dd> for the description. For additional styling options, take a look at the Description List component.

PREVIEW
MARKUP
Description lists
A description list defines terms and their corresponding descriptions.
This is a term
This is a description.
This is a term
This is a description.
Horizontal rule
<dl>
    <dt>Description lists</dt>
    <dd>A description list defines terms and their corresponding descriptions.</dd>
    <dt>This is a term</dt>
    <dd>This is a description.</dd>
    <dt>This is a term</dt>
    <dd>This is a description.</dd>
</dl>

Create a horizontal rule by using the <hr> element. For additional styling options, take a look at the Divider component.

PREVIEW
MARKUP
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.


<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>

<hr>

<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>


Blockquote
To quote multiple lines of content from another source within your document, use the <blockquote> element.

PREVIEW
MARKUP
The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a footer or cite element.

Someone famous in Source Title
Preformatted text
For multiple lines of code, use the <pre> element. It creates a new text block that preserves spaces, tabs and line breaks. Nest a <code> element inside to define the code block.

NOTE Be sure to escape any angle brackets to make sure enclosed code is not interpreted as markup.


<blockquote cite="#">
    <p class="uk-margin-small-bottom">The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a footer or cite element.</p>
    <footer>Someone famous in <cite><a href="#">Source Title</a></cite></footer>
</blockquote>


PREVIEW
MARKUP
// Code example
<div id="myid" class="myclass" hidden>
    Lorem ipsum <strong>dolor</strong> sit amet, consectetur adipiscing elit.
</div>

<pre><code>// Code example
&lt;div id="myid" class="myclass" hidden&gt;
    Lorem ipsum &lt;strong&gt;dolor&lt;/strong&gt; sit amet, consectetur adipiscing elit.
&lt;/div&gt;</code></pre>
