

Icon
Place scalable vector icons anywhere in your content.

UIkit comes with its own SVG icon system and a comprehensive library, which comprises a growing number of elegant outline icons. This component injects SVGs into the site, so that they adopt color and can be styled with CSS.

Usage
Make sure to include the icon library script, for more details see the installation instructions.

<script src="uikit/dist/js/uikit-icons.min.js"></script>
To apply this component, add the uk-icon attribute to a <span> or <a> element. To display the actual icon, you need to append the icon: NAME parameter to the attribute. Et voilà, you have a vector icon which inherits color just like your text does.

<span uk-icon="icon: check"></span>

<a href="" uk-icon="icon: heart"></a>
If icon is the only option in the attribute value, you can also use uk-icon="NAME"

<span uk-icon="heart"></span>
PREVIEW
MARKUP
 
Library
Here is an overview of all currently available icons. Over time, we will keep adding new icons to the list.

App
 home
 sign-in
 sign-out
 user
 users
 lock
 unlock
 settings
 cog
 nut
 comment
 commenting
 comments
 hashtag
 tag
 cart
 credit-card
 mail
 receiver
 search
 location
 bookmark
 code
 paint-bucket
 camera
 bell
 bolt
 star
 heart
 happy
 lifesaver
 rss
 social
 git-branch
 git-fork
 world
 calendar
 clock
 history
 future
 pencil
 trash
 move
 link
 question
 info
 warning
 image
 thumbnails
 table
 list
 menu
 grid
 more
 more-vertical
 plus
 plus-circle
 minus
 minus-circle
 close
 check
 ban
 refresh
 play
 play-circle
Devices
 tv
 desktop
 laptop
 tablet
 phone
 tablet-landscape
 phone-landscape
Storage
 file
 copy
 file-edit
 folder
 album
 push
 pull
 server
 database
 cloud-upload
 cloud-download
 download
 upload
Direction
 reply
 forward
 expand
 shrink
 arrow-up
 arrow-down
 arrow-left
 arrow-right
 chevron-up
 chevron-down
 chevron-left
 chevron-right
 triangle-up
 triangle-down
 triangle-left
 triangle-right
Editor
 bold
 italic
 strikethrough
 video-camera
 quote-right
Brands
 500px
 behance
 dribbble
 facebook
 flickr
 foursquare
 github
 github-alt
 gitter
 google
 google-plus
 instagram
 joomla
 linkedin
 pagekit
 pinterest
 soundcloud
 tripadvisor
 tumblr
 twitter
 uikit
 vimeo
 whatsapp
 wordpress
 xing
 yelp
 youtube
Ratio
Add the ratio: 2 parameter to the uk-icon attribute to double its size – or any other number, depending on how big you want you icon to be.

<span uk-icon="icon: check; ratio: 2"></span>
PREVIEW
MARKUP
 
Link modifier
To reset the default link styling to a more muted color when using an icon inside an anchor, add the .uk-icon-link class.

<a href="" class="uk-icon-link" uk-icon="heart"></a>
PREVIEW
MARKUP
  
Button modifier
Use the modifier .uk-icon-button class on an <a> element to create an icon button, which can be used for social icons.

<a href="" class="uk-icon-button" uk-icon="twitter"></a>
PREVIEW
MARKUP
  
Image modifier
You can also make any background image scale to the size of an icon. Just add the .uk-icon-image class and a background image path.

PREVIEW
MARKUP
Component options
Any of these options can be applied to the component attribute. Separate multiple options with a semicolon. Learn more

OPTION	VALUE	DEFAULT	DESCRIPTION
icon	String	''	The icon to display.
ratio	Number	1	The icon size ratio.
icon is the Primary option and its key may be omitted, if it's the only option in the attribute value.

<span uk-icon="heart"></span>
JavaScript
Learn more about JavaScript components.

Initialization
UIkit.icon(element, options);
Properties
svg
A JavaScript Promise that will resolve with the added SVG Node.

UIkit.icon(element).svg.then(function(svg) { svg.querySelector('path').style.stroke = 'red'; })
