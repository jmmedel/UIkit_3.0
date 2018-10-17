


Comment
Includes styles for comments, for example for a blog section on your site.

Usage
The Comment component consists of the comment itself, a comment header, including an avatar, a title and meta data, and a comment body.

CLASS	DESCRIPTION
.uk-comment	Add this class to define the Comment component.
.uk-comment-body	Add this class to create a comment body.
.uk-comment-header	Add this class to create a comment header.
.uk-comment-title	Add this class to a heading to create a comment title.
.uk-comment-meta	Add this class to create meta data about your comment, e.g. a subnav.
.uk-comment-avatar	Add this class to an <img> element to create an avatar for the comment author.
<article class="uk-comment">
    <header class="uk-comment-header">
        <img class="uk-comment-avatar" src="" alt="">
        <h4 class="uk-comment-title"></h4>
        <ul class="uk-comment-meta uk-subnav"></ul>
    </header>
    <div class="uk-comment-body"></div>
</article>
PREVIEW
MARKUP

Author
12 DAYS AGO
REPLY
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

Primary modifier
To style a comment differently, for example to highlight it as the admin's comment, just add the .uk-comment-primary class.

<article class="uk-comment uk-comment-primary">...</article>
PREVIEW
MARKUP

Author
12 DAYS AGO
REPLY
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

Lists
Add the .uk-comment-list class to a <ul> element to create a list of comments. You can nest any number of <ul> elements inside a comment list.

<ul class="uk-comment-list">
    <li>
        <article class="uk-comment">...</article>
        <ul>
            <li>
                <article class="uk-comment">...</article>
            </li>
        </ul>
    </li>
</ul>
PREVIEW
MARKUP

Author
12 days ago

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.


Author
12 days ago

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.


Author
12 days ago

Reply
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

