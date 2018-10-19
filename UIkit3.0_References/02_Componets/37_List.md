


List
Easily create nice looking lists, which come in different styles.

Usage
To apply this component, add the .uk-list class to an unordered or ordered list. The list will now display without any spacing or list-style.

<ul class="uk-list">
    <li></li>
    <li></li>
    <li></li>
</ul>
PREVIEW
MARKUP
List item 1
List item 2
List item 3


<ul class="uk-list">
    <li>List item 1</li>
    <li>List item 2</li>
    <li>List item 3</li>
</ul>


Bullet modifier
Add the .uk-list-bullet class to display bullets in front of the list items.

<ul class="uk-list uk-list-bullet">...</ul>
PREVIEW
MARKUP
List item 1
List item 2
List item 3

<ul class="uk-list uk-list-bullet">
    <li>List item 1</li>
    <li>List item 2</li>
    <li>List item 3</li>
</ul>


Divider modifier
Add the .uk-list-divider class to separate list items with lines.

<ul class="uk-list uk-list-divider">...</ul>
PREVIEW
MARKUP
List item 1
List item 2
List item 3

<ul class="uk-list uk-list-divider">
    <li>List item 1</li>
    <li>List item 2</li>
    <li>List item 3</li>
</ul>



Striped modifier
Add zebra-striping to a list using the .uk-list-striped class.

<ul class="uk-list uk-list-striped">...</ul>
PREVIEW
MARKUP
List item 1
List item 2
List item 3


<ul class="uk-list uk-list-striped">
    <li>List item 1</li>
    <li>List item 2</li>
    <li>List item 3</li>
</ul>


Large modifier
Add the .uk-list-large class to increase the spacing between list items. You can combine this with any of the other list modifiers.

<ul class="uk-list uk-list-large">...</ul>
PREVIEW
MARKUP
Default
List item 1
List item 2
List item 3
Divider
List item 1
List item 2
List item 3
Striped
List item 1
List item 2
List item 3
Bullet
List item 1
List item 2
List item 3


<div class="uk-child-width-expand@s" uk-grid>

    <div>
        <h4>Default</h4>
        <ul class="uk-list uk-list-large">
            <li>List item 1</li>
            <li>List item 2</li>
            <li>List item 3</li>
        </ul>
    </div>

    <div>
        <h4>Divider</h4>
        <ul class="uk-list uk-list-large uk-list-divider">
            <li>List item 1</li>
            <li>List item 2</li>
            <li>List item 3</li>
        </ul>
    </div>

    <div>
        <h4>Striped</h4>
        <ul class="uk-list uk-list-large uk-list-striped">
            <li>List item 1</li>
            <li>List item 2</li>
            <li>List item 3</li>
        </ul>
    </div>

    <div>
        <h4>Bullet</h4>
        <ul class="uk-list uk-list-large uk-list-bullet">
            <li>List item 1</li>
            <li>List item 2</li>
            <li>List item 3</li>
        </ul>
    </div>

</div>


