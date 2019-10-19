# `AppLSAC_simple_editor`
This is a simple editor for text files to show the basic principles of an [AppLSAC](https://en.wikiversity.org/wiki/AppLSAC) as a WebApp that runs completely offline in browser as runtime environment.


## Tool Chain for `AppLSAC_simple_editor`
* [`AppLSAC_simple_editor`](https://niebert.github.com/AppLSAC_simple_editor) was created with with [`JSONEditor4Menu`](https://niehausbert.gitlab.io/jsoneditor4menu)
* [`JSONEditor4Menu`](https://niehausbert.gitlab.io/jsoneditor4menu) uses [`hamburger_menu_app`](https://niebert.github.io/hamburger_menu_app) as template for the AppLSAC generation. The [`hamburger_menu_app`](https://niebert.github.io/hamburger_menu_app) contains files that are dynamically replaced by content in [`JSONEditor4Menu`](https://niehausbert.gitlab.io/jsoneditor4menu) to create individualized WebApp with a specific menu.
* [`hamburger_menu_app`](https://niebert.github.io/hamburger_menu_app) uses [Icons4Menu](https://www.github.com/niebert/icons4menu) to display icons in the Hamburger Menu of [`hamburger_menu_app`](https://niebert.github.io/hamburger_menu_app)


## Hamburger Menu Template -  Brown
The [`AppLSAC_simple_editor`](https://niebert.github.com/AppLSAC_simple_editor) is based on [`hamburger_menu_app`](https://niebert.github.io/hamburger_menu_app) as template.
The repository [`hamburger_menu_app`](https://niebert.github.io/hamburger_menu_app) contains an example of an webbased application (see [AppLSAC](https://en.wikiversity.org/wiki/WebApps_with_LocalStorage_and_AppCache)). Navigation is implemented with Hamburger Menu and JQUery.
* The folder was used for building a ZIP for the demo,
* the ZIP file [`hamburger_menu_app.zip`](https://github.com/niebert/hamburger_menu_app/archive/master.zip) was generated with a test version of [JSONEditor4Menu](https://niebert.github.io/hamburger-menu-creator) and this repository is a template ZIP for the generated ZIP file the user menu.


   <h3>Hamburger Menu App Demo: https://niebert.github.io/hamburger_menu_app </h3>

## 

## Generation of HTML, CSS and Javascript with [Handlebars4Code](https://niebert.github.io/Handlebars4Code)
The underlying concept of all code generation is a template engine [Handlebars4Code](https://niebert.github.io/Handlebars4Code), which is based on [HandleBars](http://handlebarsjs.com/) was used as template engine with additional helper functions for code generation. The [`hamburger-menu-creator`](https://niebert.github.io/hamburger-menu-creator) was build
* [`hamburger-menu-creator`](https://github.com/niebert/hamburger-menu-creator/tree/master/docs/tpl) uses the `docs/tpl/javascript_tpl.js` as template to generate the  `docs/js/menu.js` for the [<kbd>hamburger_menu_app</kbd>](https://niebert.github.io/hamburger_menu_app).
* [`hamburger-menu-creator`](https://github.com/niebert/hamburger-menu-creator/tree/master/docs/tpl) uses the `docs/tpl/css_tpl.js` as template to generate the  style sheet `docs/css/style.css` for the [<kbd>hamburger_menu_app</kbd>](https://niebert.github.io/hamburger_menu_app).
* [`hamburger-menu-creator`](https://github.com/niebert/hamburger-menu-creator/tree/master/docs/tpl) uses the `docs/tpl/html_tpl.js` as template to generate the  style sheet `docs/index.html` for the [<kbd>hamburger_menu_app</kbd>](https://niebert.github.io/hamburger_menu_app).

Code generation is performed with [Handlebars4Code](https://niebert.github.io/Handlebars4Code).

## Icons4Menu
A generic repository for menu icons is maintained in the repository [icons4menu](https://www.github.com/niebert/icons4menu). The script `update_wget_icons.sh` updates the script from the [icons4menu](https://www.github.com/niebert/icons4menu) and replaces the script `wget_icons.sh`. The script `wget_icons.sh` can be used to download an updated version of the icons. Please modify the script according to your needs, to download just a subset for your [AppLSAC](https://en.wikiversity.org/wiki/WebApps_with_LocalStorage_and_AppCache).


## Change Log
* Version 3.1.0 [Icons4Menu](https://www.github.com/niebert/icons4menu) icons updated in folder `/img` - with `sh update_wget_icons.sh` and `sh wget_icons.sh` - see repository https://niebert.github.io/icons4menu for licencsing details for the icons.
* Version 3.0.0 [Icons4Menu](https://www.github.com/niebert/icons4menu) is used to display icons - see repository https://niebert.github.io/icons4menu for licencsing details for the icons.
* Version: 2.0.0 Font Awesome dependency removed - [JQuery Icons](https://jqueryui.com) used for icons in the menu. The folder `img/` contains the folder with JQuery icons in `PNG` and `SVG` format that can be used directly in the HTML file by embedding them with `IMG` tags in HTML. This is a robost method to have the icons of choice available for the developers.
* Version 1.0.0: Was dependent on [Font Awesome Icons - 4.7.0](https://fontawesome.com/v4.7.0/icons/) used for icons in the Hamburger menu

## Acknowledgement
Special thanks to the following individual developers and teams of OpenSource JavaScript projects:
* [JQuery](https://jqueryui.com) is used for the theme and standard operations in the Document Object Model (DOM) of HTML-pages. The [JQuery-Themeroller](https://jqueryui.com/themeroller/) was used to create a JQuery theme for JSCC.
* [Font Awesome Icons - 4.7.0](https://fontawesome.com/v4.7.0/icons/) thanks to [fontawesome.com](https://fontawesome.com) for providing the [free 4.7.0 version](https://fontawesome.com/v4.7.0/icons/) for local application for this WebApp. The [fonts in version 4.7.0](https://fontawesome.com/v4.7.0/icons/) are created by ***[Font Awesome](https://fontawesome.com)*** and
licensed under [SIL OFL 1.1](http://scripts.sil.org/OFL). The javascript-code for injecting the icon into the DOM licensed under [MIT License](http://opensource.org/licenses/mit-license.html). The
[Documentation](https://fontawesome.com/v4.7.0/examples/) for [Font Awesome - 4.7.0](https://fontawesome.com/v4.7.0/icons/) licensed under [CC BY 3.0](http://creativecommons.org/licenses/by/3.0/). The [Font-Awesome GitHub-repository](https://github.com/FortAwesome/Font-Awesome) can be used for forking and adapting the javascript code to individual requirements and constraints.
* [HandleBars](http://handlebarsjs.com/) was used as template engine in Javascript
* [JSON-Editor](https://github.com/jdorn/json-editor) by Jeremy Dorn. The JSON Editor takes a JSON Schema and uses it to generate an HTML form. The JSON-Editor is partially used to edit JSON file of the [JavascriptClassCreator Project](https://niebert.github.io/JavascriptClassCreator) `JSCC`.
The JSON-Editor of Jeremy Dorn has full support for JSON Schema version 3 and 4 and can integrate with several popular CSS frameworks (bootstrap, foundation, and jQueryUI). This would lead to major code reduction of `JSCC` . Refactoring of `JSCC` would make more use of the JSON-Editor features. Check out an interactive demo (demo.html): http://jeremydorn.com/json-editor/
* Developer [Mihai Bazon](http://lisperator.net/) create UglifyJS, a great tool to handle and parse Javascript Code and minify the Javascript code (see [Source Code of UglifyJS](https://github.com/mishoo/UglifyJS2)).
* The wrapper for UglifyJS is written [Dan Wolff](http://danwolff.se/). His UglifyJS-Online example is used to minify/compress the exported Javascript code of generated JS Classes (For Online Example of the [UglifyJS-Wrapper](https://skalman.github.io/UglifyJS-online/) see source code on https://github.com/Skalman/UglifyJS-online for the Online-Version of the Wrapper.
* Developers of ACE Code Editor https://ace.c9.io (Javascript Editing uses the Editor in iFrames)
* [FileSaver.js](https://github.com/eligrey/FileSaver.js) Developer Eli Grey provided the `FileSaver.js` that is used to store created `JSCC` files to the local filesystem. `JSCC` uses the same mechanism of browsers, that allows a `Save as...` in the context menu of a web pages or image. So not uncontrolled write access to your file system is implemented, because users have to select the locations in which the user whats to store the file (e.g. JSON, Javascript or HTML).
* [JointJS](https://github.com/clientIO/joint) JointJS is a JavaScript diagramming library. It can be used to create either static diagrams. JointJS is used in this project to create UML-diagrams, that are interactive diagramming in conjunction and application builder in Javascript.
* [Inheritage for JavaScript with protoypes](http://phrogz.net/js/classes/OOPinJS2.html) by Gavin Kistner
* [3 ways to define a JavaScript class](https://www.phpied.com/3-ways-to-define-a-javascript-class/) by Stoyan Stefanov
