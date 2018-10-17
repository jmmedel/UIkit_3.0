


Form
Easily create nice looking forms with different styles and layouts.

Usage
Add one of the following classes to form controls inside a <form> element to define them.

CLASS	DESCRIPTION
.uk-input	Add this class to <input> elements.
.uk-select	Add this class to <select> elements.
.uk-textarea	Add this class to <textarea> elements.
.uk-radio	Add this class to <input type="radio"> elements to create radio buttons.
.uk-checkbox	Add this class to <input type="checkbox"> elements to create checkboxes.
.uk-range	Add this class to <input type="range"> elements to create range forms.
<form>
    <select class="uk-select">
        <option></option>
        <option></option>
    </select>
    <textarea class="uk-textarea"></textarea>
    <input class="uk-radio" type="radio">
    <input class="uk-checkbox" type="checkbox">
    <input class="uk-range" type="range">
</form>
Add the .uk-fieldset class to a <fieldset> element and the .uk-legend class to a <legend> element to define a fieldset and a form legend.

PREVIEW
MARKUP
Legend

Input
 

Textarea
  A
 B
 A
 B

States modifiers
Provide the user with basic information through feedback states on form controls by using one of the following classes.

CLASS	DESCRIPTION
.uk-form-danger	Add this class to notify the user that the value is not validated.
.uk-form-success	Add this class to notify the user that the value is validated.
Add the disabled attribute to a form control and it will be appear muted.

PREVIEW
MARKUP

form-danger
 
form-success
 
disabled
Size modifiers
Add one of the classes to an <input>, <select> or <textarea> element to modify its size.

CLASS	DESCRIPTION
.uk-form-large	Add this class to make the element larger.
.uk-form-small	Add this class to make the element smaller.
PREVIEW
MARKUP

Large
 
Default
 
Small
Width modifiers
Add one of the following classes to an <input>, <select> or <textarea> element to adjust its width.

CLASS	DESCRIPTION
.uk-form-width-large	Applies a width of 500px.
.uk-form-width-medium	Applies a width of 200px.
.uk-form-width-small	Applies a width of 130px.
.uk-form-width-xsmall	Applies a width of 40px.
PREVIEW
MARKUP

Large
 
Medium
 
Small
 
XSmall
You can also apply the .uk-width-* classes from the Width component to form controls.

PREVIEW
MARKUP

uk-width-1-2
Blank modifier
Add the .uk-form-blank class to minimize the styling of form controls.

PREVIEW
MARKUP

Form blank
Layout
Define labels and controls and apply a stacked or horizontal layout to form elements. Layout modifiers can be added to any parent element like the <fieldset> element. This makes it possible to have different form layouts for each fieldset.

CLASS	DESCRIPTION
.uk-form-stacked	Add this class to display labels on top of controls.
.uk-form-horizontal	Add this class to display labels and controls side by side.
.uk-form-label	Add this class to define form labels.
.uk-form-controls	Add this class to define form controls.
<form class="uk-form-stacked">
    <div>
        <label class="uk-form-label"></label>
        <div class="uk-form-controls">...</div>
    </div>
    <div>
        <div class="uk-form-label"></div>
        <div class="uk-form-controls">...</div>
    </div>
</form>
PREVIEW
MARKUP
Text

Some text...
Select

Radio
 Option 01
 Option 02
Horizontal form
Use the .uk-form-controls-text class to better align checkboxes and radio buttons when using them with text in a horizontal layout.

<form class="uk-form-horizontal">
    <div>
        <label class="uk-form-label"></label>
        <div class="uk-form-controls">...</div>
    </div>
    <div>
        <div class="uk-form-label"></div>
        <div class="uk-form-controls uk-form-controls-text">...</div>
    </div>
</form>
PREVIEW
MARKUP
Text

Some text...
Select

Radio
 Option 01
 Option 02
Form and icons
You use an icon from the Icon component inside a form. Add the .uk-form-icon class to a <span> element. Group it with an <input> element by adding the .uk-inline class from the Utility component to a container element around both. The icon has to come first in the markup. By default, the icon will be placed on the left side of the form. To change the alignment, add the .uk-form-icon-flip class.

<div class="uk-inline">
    <span class="uk-form-icon" uk-icon="icon: user"></span>
    <input class="uk-input">
</div>
PREVIEW
MARKUP

 
Clickable icons
To enable an action, for example opening a modal to pick an image or link, use an <a> or <button> element to create the icon.

<div class="uk-inline">
    <a class="uk-form-icon uk-form-icon-flip" href="" uk-icon="icon: user"></a>
    <input class="uk-input">
</div>
PREVIEW
MARKUP

 
Form and grid
You can also use the Grid and Width components to define the layout of a form.

PREVIEW
MARKUP

100
 
50
 
25
 
25
 
50
 
50
Custom controls
To replace a file inputs or select forms with your own HTML content, like a button or text, add the uk-form-custom attribute to a container element.

File
Use a button or text as a file input.

<div uk-form-custom>
    <input type="file">
    <button type="button"></button>
</div>
PREVIEW
MARKUP
SELECT
Here is a text  upload

Select file
  SUBMIT
Select
Use a button, text or a link as a select form. Just add the target: SELECTOR option to the uk-form-custom attribute to select where the option value should be displayed. target: true will select the adjacent element in the markup.

<div uk-form-custom="target: true">
    <select>
        <option></option>
        <option></option>
    </select>
    <button type="button"></button>
</div>
PREVIEW
MARKUP
Option 01
 Option 01
PLEASE SELECT... 
Component option
You can add this option to the uk-form-custom attribute. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
target	CSS selector, Boolean	false	Value display target.
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.formCustom(element, options);

