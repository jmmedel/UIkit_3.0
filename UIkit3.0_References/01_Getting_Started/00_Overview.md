

# The Oficial website for UIkit3.0 
https://getuikit.com

Introduction
Get familiar with the basic setup and overview of UIkit.

First of all you need to download UIkit. For other packages and links to a CDN, head to the installation guide to learn more.

DOWNLOAD UIKIT

Package contents
The Zip file contains the compiled CSS and JavaScript files, which is everything you need to get started. Later, you might want to install and compile UIkit yourself and also create your own UIkit theme.

FOLDER	DESCRIPTION
/css	Contains the UIkit CSS and a right-to-left version.
/js	Contains the UIkit JavaScript and the Icon Library JavaScript.
HTML markup
Add the compiled and minified CSS and JavaScript to the <head> element of your HTML5 document. Also include the UIkit icon library. For your basic setup, that's it.

<!DOCTYPE html>
<html>
    <head>
        <title>Title</title>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link rel="stylesheet" href="css/uikit.min.css" />
        <script src="js/uikit.min.js"></script>
        <script src="js/uikit-icons.min.js"></script>
    </head>
    <body>
    </body>
</html>
Once you have included UIkit into your document, take a look at the available components and create your own markup inside the <body> element of your page.

UIkit autocomplete for your editor
Using UIkit works best if you have a solid code editor, for example Sublime Text or Atom. To be even more efficient, we recommend that you install one of the autocomplete plugins for your favorite IDE or code editor. This saves a lot of time, as you won't have to look up and type all UIkit classes and markup.

Autocomplete plugin for Sublime Text 3
Autocomplete plugin for Atom
Browser support
The following table lists the versions that UIkit is tested on. "Latest" means that it works just fine on all recent versions of that browser. With many browser moving towards a rolling release strategy, pinning down browser support to a specific version has become a little tricky in recent years. Long story short: UIkit will work on pretty much any modern browser.


