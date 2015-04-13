# Swill Boilerplate

![Swill Boilerplate Logo](https://raw.githubusercontent.com/tiagoporto/swill-boilerplate/stylus-version/src/images/touch/chrome-touch-icon-192x192.png)

Boilerplate Front-End with [Gulp.js](http://gulpjs.com/), all you need to start multi-device development for business proposals, easy to customize.

## Table of Contents

* [Version](#versions)
* [Technologies](#technologies)
* [Includes](#includes)
* [Features](#features)
* [Folder Structure](#folder-structure)
* [Installing Dependencies](#installing-dependencies)
* [Usage](#usage)
	* [Tasks](#tasks)
	* [Peculiarities](#peculiarities)
	* [AngulaJS](#angularjs)
	* [BrowserSync](#browsersync)
	* [Bitmap Sprite](#sprite)
	* [SVG Sprite](#svg*sprite)
* [License](license)

## Versions

> [Sass Version](https://github.com/tiagoporto/swill-boilerplate/tree/sass-version).
>
> If you're like me and prefer stylus as pre-processor use the [Stylus Version](https://github.com/tiagoporto/swill-boilerplate/tree/stylus-version).
>
> If you will work with Ionic you use the [Mobile Version](https://github.com/tiagoporto/swill-boilerplate/tree/mobile-version).
>
> [Light version](https://github.com/tiagoporto/swill-boilerplate/tree/stylus-version-light)

## Technologies

Uses the following technologies:

* [Autoprefixer](https://github.com/postcss/autoprefixer)
* [Bower](http://bower.io/)
* [BrowserSync](http://www.browsersync.io/)
* [EditorConfig](http://editorconfig.org/)
* [Gulp.js](http://gulpjs.com/)
* [JSHint](http://www.jshint.com/)
* [Node.js](http://nodejs.org/)
* [NPM](https://www.npmjs.com/)
* [Sass](http://sass-lang.com/) or [Stylus](http://learnboost.github.io/stylus/)

## Includes

* [AngularJS](http://angularjs.org/)
* [Animate.css](http://daneden.github.io/animate.css/)
* [Font Awesome](http://fortawesome.github.io/Font-Awesome/)
* [Google Analytics](http://www.google.com/analytics/)
* [jQuery](http://jquery.com/)
* [Normalize.css](http://necolas.github.io/normalize.css/)
* [Outdated Browser](http://outdatedbrowser.com/)
* [Retina.js](http://imulus.github.io/retinajs/)
* [Semantic GRID SYSTEM](http://semantic.gs/)
* [Twitter Bootstrap](http://getbootstrap.com/)

## Features

* Clean the assets (images, css, js) in the project to maintain the directory organized
* Compress Images
* Generate Sprites with .png
* Generate Sprites with .svg and a fallback .png
* Concatenate And Minify Scripts
* Analyze JavaScript with jshint
* Compile Sass or Stylus
* Catch the stylus error and direct shows on the page, as in sass.
* Functions and mixins to use with Sass or Stylus
* Notify when tasks are complete
* Monitors changes in the files and reload browser with [BrowserSync](http://www.browsersync.io/)
* Configs from [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate)
* Check if the browser is outdated with [Outdated Browser](http://outdatedbrowser.com/)
* Build the project compressing the HTML and the CSS.


## Folder Structure

```
./
├──┐
│  ├─ node_modules // Will appear after installed the NPM packages
│  │  └─ // NPM packages
│  │
│  ├─ build // Folder with the builded project
│  │
│  ├─ public // Files for deployment
│  │  ├─ css
│  │  │  └─ // Public styles
│  │  │
│  │  ├─ fonts
│  │  │  └─ // Web Fonts
│  │  │
│  │  ├─ images
│  │  │  │
│  │  │  ├─ copyright // Images with copyright metadata
│  │  │  │
│  │  │  ├─ logos // Logos
│  │  │  │
│  │  │  └─ // Public images
│  │  │
│  │  ├─ js
│  │  │  └─ // Public scripts
│  │  │
│  │  ├─ lang
│  │  │  ├─ outdated_browser // Langs to outdated browser plugin
│  │  │  │
│  │  │  │
│  │  │  └─ // Langs to multilingue sites
│  │  │
│  │  ├─ .htaccess // Configuration for use on web servers running the Apache Web Server
│  │  │
│  │  ├─ 404.html // Page to 404 error
│  │  │
│  │  ├─ apple-touch-icon.png // Icon for Safari on iOS
│  │  │
│  │  ├─ crossdomain.xml // Permission to handle data across multiple domains
│  │  │
│  │  ├─ example.html // Simple page with example of the components
│  │  │
│  │  ├─ favicon.ico //Icon for address bar and bookmark
│  │  │
│  │  ├─ index.html
│  │  │
│  │  ├─ manifest.json //Provides information about an Chrome app https://developer.chrome.com/extensions/manifest
│  │  │
│  │  ├─ manifest.webapp //Provides information about an Firefox OS app https://developer.mozilla.org/pt-BR/Apps/Manifest
│  │  │
│  │  ├─ robots.txt //Give instructions about their site to search engines
│  │  │
│  │  └─ // HTML, PHP, etc Files
│  │
│  └─ src // Source files for the projects
│       ├─ images // Original imagens, don't compressed
│       │  │
│       │  ├─ sprite // Images to generate the sprite
│       │  │
│       │  ├─ svg-sprite // Svgs to generate the svg-sprite
│       │  │
│       │  └─ touch // Icons
│       │      │
│       │      ├─ chrome-touch-icon-192x192.png // Icon for Chrome on Android
│       │      │
│       │      ├─ icon-128x128.png // Icon for Firefox on FirefoxOS
│       │      │
│       │      ├─ tile.png // Tile icon for Win8
│       │      │
│       │      ├─ tile-wide.png // Wide tile icon for Win8
│       │      │
│       │      └─ // .jpg, .jpeg, .gif, .svg and .bmp to be compressed
│       │
│       ├─ scripts
│       │  │
│       │  ├─ angular // Development with AngularJS
│       │  │
│       │  ├─ dependencies // External plugins
│       │  │
│       │  ├─ jquery
│       │  │  │
│       │  │  ├─ onread // Open and close on read of Jquery
│       │  │  │
│       │  │  └─ // Development with JQuery
│       │  │
│       │  ├─ settings
│       │  │  │
│       │  │  ├─ call_plugins.js // Call the plugins after page load
│       │  │  │
│       │  │  └─ google_analytics.js // Settings to Analytics
│       │  │
│       │  └─ // Development with Pure Javascript
│       │
│       └─ stylesheets
│            │
│            ├─ components //Styles used by external plugins
│            │
│            ├─ dependencies //Styles used by external plugins
│            │
│            ├─ helpers
│            │  │
│            │  ├─ functions
│            │  │  │
│            │  │  └ //
│            │  │
│            │  ├─ mixins
│            │  │  │
│            │  │  └ //
│            │  │
│            │  ├─ _functions.{sass, styl}
│            │  │
│            │  ├─ _helpers.{sass, styl}
│            │  │
│            │  ├─ _mixins.{sass, styl}
│            │  │
│            │  ├─ _placeholders.{sass, styl}
│            │  │
│            │  ├─ _sprite.{sass, styl}
│            │  │
│            │  ├─ _svg-sprite.{sass, styl}
│            │  │
│            │  └─ _variables.{sass, styl}
│            │
│            ├─ media_queries
│            │
│            ├─ typography
│            │
│            ├─ _base.{sass, styl} // Main Styles
│            │
│            └─ styles.{sass, styl} // Base file with imports
│
├─ .editorconfig // Settings of editorconfig plugin
├─ .jshintrc // JSHint configuration file
├─ bower.json // Bower dependencies
├─ gulpfile.js // Gulp.js configuration file
├─ package.json // NPM dependencies
└─ README.md // Documentation
```

## Installing Dependencies

1. Install [EditorConfig](http://editorconfig.org/)

	* Download and install the [EditorConfig plugin](http://editorconfig.org/#download) for you text editor.

1. Download and install [Node.js](http://nodejs.org/download/)

	`Select npm package manager`


1. Install [Gulp.js](http://gulpjs.com/)

	* Open command line and execute

	```sh
	$ npm install gulp -g
	```

	For Mac or Linux User

	```sh
	$ sudo npm install gulp -g
	```

1. Install [Bower](http://bower.io/)

	* Execute

	```sh
	$ npm install -g bower
	```

> Necessary just to sass-version and mobile-version.

1. In Windows is necessary install [Ruby](https://www.ruby-lang.org/)

	* Download and install [Ruby](http://rubyinstaller.org/).

1. Install Gem [Sass](http://sass-lang.com/)

	* Open command line and execute

	```sh
	$ gem install sass
	```


## Usage

1. Install [NPM](https://www.npmjs.com/) dependencies

	* In the command line go to the local folder

	```sh
	$ cd {yourFolderStructure}/swill-boilerplate
	```

	* Execute

	```sh
	$ npm install
	```

1. Open the file `bower.json`
	* Remove the dependencies that you will not use.

1. Open the command line
	* Go to the local folder

	```sh
	$ cd {yourFolderStructure}/swill-boilerplate
	```

1. Install [Bower](http://bower.io/) Dependencies
	* Execute

	```sh
	$ bower install
	```

	```sh
	$ gulp bower
	```

1. Execute the task `gulp` to start the development

```sh
$ gulp
```

### Tasks

**Default Task** - compile, watch and serve project.

```sh
$ gulp
```

**Compile Task** - just compile project.

```sh
$ gulp compile
```

**Serve Task** - serve the project and watch.

```sh
$ gulp serve
```

**Build Task** - build project.

```sh
$ gulp build
```

**Build:serve task** - build and serve builded project.

```sh
$ gulp build:serve
```

### Peculiarities

* Js Files prefixed with `_` won't be concatenated.

* The folder `public/img` is clean when the task is run, and the images are compressed and come from ` src/images`, but if you work with copyrighted images you should not use compression, because it removes the metadatas from files. You can place images direct in the `public/src/copyright`, they won't be deleted.

> If for some other reason you want to use other folders directly in the `public/img`, add the folder in the task ` clean` on `gulpfile.js`, and it won't be deleted.

* To use bower components just link the file on the HTML inside of the especifics comments. This way all the files will be concatenated and minified to build.

**Example**

```html
	<!-- build:js js/scripts.min.js -->
	<script src="angular/angular.js"></script>
	<script src="angular-route/angular-route.js"></script>
	<script src="js/main.js"></script>
	<!-- endbuild -->
```

*The link to file start inside of the `bower_components`, the application won't work out of the serve.*


### AngulaJS

To use Angular go to the `gulpfile.js` uncomment the lines with `mangle: false`.


### BrowserSync

If you will work with dinamic files like .php, it's necessary make changes in `gulpfile.js` to BrowserSync works

Remove the lines
```javascript
server: {
	baseDir: [basePaths.src, basePaths.dest]
}
```
Set the url to the server
```javascript
proxy: "localhost/swill-boilerplate/public/"
```

### Bitmap Sprite

This boilerplate uses [gulp.spritesmith](https://www.npmjs.org/package/gulp.spritesmith) to generate bitmap sprites.

When the sprite is generated, a file `_sprite.styl` or `_sprite.sass` is created with four mixins and the variables of the parameters of the images, like height and width (the names of the variables is the same of the original filename before the compilation).

**Sprite file example**

```styl

$left-arrow-x: 0px;
$left-arrow-y: 0px;
$left-arrow-offset-x: 0px;
$left-arrow-offset-y: 0px;
$left-arrow-width: 32px;
$left-arrow-height: 32px;
$left-arrow-total-width: 32px;
$left-arrow-total-height: 66px;
$left-arrow-image: '../images/sprite.png';

@mixin sprite-width($sprite) {
  width: nth($sprite, 5);
}

@mixin sprite-height($sprite) {
  height: nth($sprite, 6);
}

@mixin sprite-position($sprite) {
  $sprite-offset-x: nth($sprite, 3);
  $sprite-offset-y: nth($sprite, 4);
  background-position: $sprite-offset-x  $sprite-offset-y;
}

@mixin sprite-image($sprite) {
  $sprite-image: nth($sprite, 9);
  background-image: url(#{$sprite-image});
}

@mixin sprite($sprite) {
  @include sprite-image($sprite);
  @include sprite-position($sprite);
  @include sprite-width($sprite);
  @include sprite-height($sprite);
}
```

Just use the mixins with the variables as parameters.

**Example**

```styl
#arrow
	sprite($left-arrow)

	&:hover
		sprite-position($right-arrow)
```

**Output**

```css
#arrow {
	background-image: url(../images/sprite.png);
	background-position: 0px 0px;
	width: 32px;
	height: 32px;
}
#arrow:hover {
	background-position: 0px -34px;
}
```

### Svg Sprite

To generate SVG sprites is used [gulp-svg-sprite](https://github.com/jkphl/gulp-svg-sprite) as fallback all the SVG sprites are converted to .png with [gulp-svg2png](https://github.com/akoenig/gulp-svg2png)

To-do

## License

Swill Boilerplate is released under the terms of the [MIT license](http://opensource.org/licenses/MIT).
