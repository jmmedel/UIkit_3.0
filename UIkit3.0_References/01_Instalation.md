
Installation
Learn where to download and how to compile the UIkit sources.

Download
You have the following options to get UIkit:

Download the latest release with pre-built JavaScript and CSS.
Install with Yarn to get the pre-built JavaScript, CSS and the Less source files. This is recommended when using UIkit for a typical web project: yarn add uikit
Clone the repo to get all source files including build scripts: git clone git://github.com/uikit/uikit.git
The compiled files of all UIkit versions are also hosted on the Cloudflare content delivery network via cdnjs.com.

<!-- UIkit CSS -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/uikit/3.0.0-rc.19/css/uikit.min.css" />

<!-- UIkit JS -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/uikit/3.0.0-rc.19/js/uikit.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/uikit/3.0.0-rc.19/js/uikit-icons.min.js"></script>
NOTE The latest Subresource Integrity (SRI) hashes can be obtained through CDNJS.

File structure of the source
The Github project contains all source files which are compiled into the dist folder. Less sources are compiled into CSS files, JavaScript sources are bundled and transpiled into ECMAScript 5 and icons are bundled into the icon library.

FOLDER	DESCRIPTION
/src	Contains all Less, JavaScript and image sources.
/dist	Contains compiled CSS and JS, updated on every release.
/tests	Contains HTML test files of all components.
Compile from Github source
To compile UIkit yourself, you can use the included build scripts.

# Run once to install all dependencies
yarn

# Compile all source files
yarn compile

# Watch files and compile automatically everytime a file changes
yarn watch
NOTE Use Node.js version 8.2.0 or higher.

The compiled dist folder now contains additional files which are not checked in by default. The build task will create even more additional files if you have added a custom UIkit theme.

/dist/css

    <!-- UIkit's CSS -->
    uikit.css
    uikit.min.css

    <!-- UIkit's core styles, without the default theme -->
    uikit-core.css
    uikit-core.min.css

    <!-- UIkit's CSS in a right-to-left version -->
    uikit.rtl.css
    uikit.rtl.min.css


/dist/js

    <!-- UIkit's JavaScript -->
    uikit.js
    uikit.min.js

    <!-- Stripped down JavaScript. Core functionality without additional components -->
    uikit-core.js
    uikit-core.min.js

    <!-- Icon Library -->
    uikit-icons.js
    uikit-icons.min.js

    <!-- Additional components (e.g. Lightbox), only needed when including uikit-core.js -->
    /components
To use UIkit's CSS and JavaScript, include the files in your own HTML and then create the markup of any of the components listed here in the docs.

To compile UIkit automatically everytime you change the LESS or JavaScript, you can use the included build scripts.

yarn watch
