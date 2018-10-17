
Close
Create a close icon that can be combined with different components.

Usage
To apply this component, add the uk-close attribute to an <a> or <button> element.

<button type="button" uk-close></button>

<a href="" uk-close></a>
PREVIEW
MARKUP

Large modifier
Add the .uk-close-large class for a larger close button.

<button class="uk-close-large" type="button" uk-close></button>
PREVIEW
MARKUP

Close in alerts
This is an example of how this component is used with an alert box from the Alert component.

<div uk-alert>
    <button class="uk-alert-close" type="button" uk-close></button>
</div>
PREVIEW
MARKUP

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.

Close in drops
This is an example of how this component is used with the Drop component.

<div uk-drop>
    <button class="uk-drop-close" type="button" uk-close></button>
</div>
PREVIEW
MARKUP
CLICK
Close in modals
This is an example of how this component is used with the Modal component.



<div class="uk-inline">
    <button class="uk-button uk-button-default" type="button">Click</button>
    <div uk-drop="mode: click">
        <div class="uk-card uk-card-body uk-card-default">
            <button class="uk-drop-close" type="button" uk-close></button>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.</p>
        </div>
    </div>
</div>



<div id="modal" uk-modal>
    <div class="uk-modal-dialog uk-modal-body">
        <button class="uk-modal-close-default" type="button" uk-close></button>
    </div>
</div>
PREVIEW
MARKUP
OPEN MODAL


<a class="uk-button uk-button-default" href="#modal" uk-toggle>Open modal</a>
<div id="modal" uk-modal>
    <div class="uk-modal-dialog uk-modal-body">
        <button class="uk-modal-close-default" type="button" uk-close></button>
        <h2 class="uk-modal-title">Headline</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        <p class="uk-text-right">
            <button class="uk-button uk-button-default uk-modal-close" type="button">Cancel</button>
            <button class="uk-button uk-button-primary" type="button">Save</button>
        </p>
    </div>
</div>





