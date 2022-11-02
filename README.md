CONTENTS OF THIS FILE

- Introduction
- Requirements
- Installation
- Configuration
- Maintainers

INTRODUCTION

The Easy Breadcrumb module provides configurable breadcrumbs that improve oncore breadcrumbs by including the current page title as an unlinked crumb whichfollows breadcrumb best-practices(URL "https://www.nngroup.com/articles/breadcrumb-navigation-useful/").Easy Breadcrumb takes advantage of the work you've already done for generatingyour path aliases, while it naturally encourages the creation of semanticand consistent paths. This module is currently available for Drupal 6.x, 7.x,and 8.x.x.

Easy Breadcrumb uses the current URL (path alias) and the current page's titleto automatically extract the breadcrumb's segments and its respective links.The module is really a plug and play module because it auto-generates thebreadcrumb by using the current URL and nothing extra is needed.

- For the description of the module visit:https://www.drupal.org/project/easy_breadcrumborhttps://www.drupal.org/docs/8/improve-the-breadcrumbs
- To submit bug reports and feature suggestions, or to track changes visit:https://www.drupal.org/node/2929013

REQUIREMENTS

This module requires no modules outside of Drupal core.

INSTALLATION

Install the Easy Breadcrumb module as you would normally install a contributedDrupal module. Visit https://www.drupal.org/node/1897420 for furtherinformation.

CONFIGURATION

    1. Navigate to Administration > Extend and enable the module. The system
       breadcrumb block has now been updated.
    2. Navigate to Administration > Configuration > User Interface > Easy
       Breadcrumb for configurations. Save Configurations.

Configurable parameters:

- Include / Exclude the front page as a segment in the breadcrumb.
- Include / Exclude the current page as the last segment in the breadcrumb.
- Use the real page title when it is available instead of always deducing itfrom the URL.
- Print the page's title segment as a link.
- Make the language path prefix a segment on multilingual sites where a pathprefix ("/en") is used.
- Use menu title as fallback instead of raw path component.
- Remove segments of the breadcrumb that are identical.
- Use a custom separator between the breadcrumb's segments. (TODO)
- Choose a transformation mode for the segments' title.
- Make the 'capitalizator' ignore some words.

MAINTAINERS

- Greg Boggs - https://www.drupal.org/u/greg-boggs
- Neslee Canil Pinto - https://www.drupal.org/u/neslee-canil-pinto
- Brooke Mahoney (loopduplicate) - https://www.drupal.org/u/loopduplicate

Supporting organization:

- Kanopi Studios - https://www.drupal.org/kanopi-studios

---



GFM  Markdown and WYSIWYG Editor - Productive and Extensible

    



🚩 Table of Contents

- Packages
- Why TOAST UI Editor?
- Features
- Examples
- Browser Support
- Pull Request Steps
- Contributing
- TOAST UI Family
- Used By
- License

📦 Packages

TOAST UI Editor

  Name            	Description               
  @toast-ui/editor	Plain JavaScript component

TOAST UI Editor's Wrappers

  Name                  	Description            
  @toast-ui/react-editor	React wrapper component
  @toast-ui/vue-editor  	Vue wrapper component  

TOAST UI Editor's Plugins

  Name                                    	Description                    
  @toast-ui/editor-plugin-chart           	Plugin to render chart         
  @toast-ui/editor-plugin-code-syntax-highlight	Plugin to highlight code syntax
  @toast-ui/editor-plugin-color-syntax    	Plugin to color editing text   
  @toast-ui/editor-plugin-table-merged-cell	Plugin to merge table columns  
  @toast-ui/editor-plugin-uml             	Plugin to render UML           

🤖 Why TOAST UI Editor?

TOAST UI Editor provides Markdown mode and WYSIWYG mode. Depending on the type of use you want like production of Markdown or maybe to just edit the Markdown. The TOAST UI Editor can be helpful for both the usage. It offers Markdown mode and WYSIWYG mode, which can be switched any point in time.

Productive Markdown Mode



CommonMark + GFM Specifications

Today CommonMark is the de-facto Markdown standard. GFM (GitHub Flavored Markdown) is another popular specification based on CommonMark - maintained by GitHub, which is the Markdown mostly used. TOAST UI Editor follows both CommonMark and GFM specifications. Write documents with ease using productive tools provided by TOAST UI Editor and you can easily open the produced document wherever the specifications are supported.

- Live Preview : Edit Markdown while keeping an eye on the rendered HTML. Your edits will be applied immediately.
- Scroll Sync : Synchronous scrolling between Markdown and Preview. You don't need to scroll through each one separately.
- Syntax Highlight : You can check broken Markdown syntax immediately.

Easy WYSIWYG Mode



- Table : Through the context menu of the table, you can add or delete columns or rows of the table, and you can also arrange text in cells.
- Custom Block Editor : The custom block area can be edited through the internal editor.
- Copy and Paste : Paste anything from browser, screenshot, excel, powerpoint, etc.

UI

- Toolbar : Through the toolbar, you can style or add elements to the document you are editing.
  
- Dark Theme : You can use the dark theme.
  

Use of Various Extended Functions - Plugins



CommonMark and GFM are great, but we often need more abstraction. The TOAST UI Editor comes with powerful Plugins in compliance with the Markdown syntax.

Five basic plugins are provided as follows, and can be downloaded and used with npm.

- chart : A code block marked as a 'chart' will render TOAST UI Chart.
- code-syntax-highlight : Highlight the code block area corresponding to the language provided by Prism.js.
- color-syntax : 
  Using TOAST UI ColorPicker, you can change the color of the editing text with the GUI.
- table-merged-cell : 
  You can merge columns of the table header and body area.
- uml : A code block marked as an 'uml' will render UML diagrams.

🎨 Features

- Viewer : Supports a mode to display only markdown data without an editing area.
- Internationalization (i18n) : Supports English, Dutch, Korean, Japanese, Chinese, Spanish, German, Russian, French, Ukrainian, Turkish, Finnish, Czech, Arabic, Polish, Galician, Swedish, Italian, Norwegian, Croatian + language and you can extend.
- Widget : This feature allows you to configure the rules that replaces the string matching to a specific RegExp with the widget node.
- Custom Block : Nodes not supported by Markdown can be defined through custom block. You can display the node what you want through writing the parsing logic with custom block.

🐾 Examples

- Basic
- Viewer
- Using All Plugins
- Creating the User's Plugin
- Customizing the Toobar Buttons
- Internationalization (i18n)

Here are more examples and play with TOAST UI Editor!

🌏 Browser Support

  Chrome	Internet Explorer	Edge	Safari	Firefox
   Yes  	       11+       	Yes 	 Yes  	  Yes  

🔧 Pull Request Steps

TOAST UI products are open source, so you can create a pull request(PR) after you fix issues. Run npm scripts and develop yourself with the following process.

Setup

Fork main branch into your personal repository. Clone it to local computer. Install node modules. Before starting development, you should check if there are any errors.

    $ git clone https://github.com/{your-personal-repo}/tui.editor.git
    $ npm install
    $ npm run build toastmark
    $ npm run test editor

TOAST UI Editor uses npm workspace, so you need to set the environment based on npm7. If subversion is used, dependencies must be installed by moving direct paths per package.

Develop

You can see your code reflected as soon as you save the code by running a server. Don't miss adding test cases and then make green rights.

Run snowpack-dev-server

snowpack allows you to run a development server without bundling.

    $ npm run serve editor

Run webpack-dev-server

If testing of legacy browsers is required, the development server can still be run using a webpack.

    $ npm run serve:ie editor

Run test

    $ npm test editor

Pull Request

Before uploading your PR, run test one last time to check if there are any errors. If it has no errors, commit and then push it!

For more information on PR's steps, please see links in the Contributing section.

💬 Contributing

- Code of Conduct
- Contributing Guideline
- Commit Convention
- Issue Guidelines

🍞 TOAST UI Family

- TOAST UI Calendar
- TOAST UI Chart
- TOAST UI Grid
- TOAST UI Image Editor
- TOAST UI Components

🚀 Used By

- NHN Dooray! - Collaboration Service (Project, Messenger, Mail, Calendar, Drive, Wiki, Contacts)
- UNOTES - Visual Studio Code Extension

📜 License

This software is licensed under the MIT © NHN Cloud.

---

React Tilt



























👀 Easily apply tilt hover effect on React components



Demo 💥

Install

    npm install react-parallax-tilt

Features

- Lightweight (≈3kB), zero dependencies 📦
- Works with React v15 onwards
- Supports mouse and touch events
- Support for device tilting (gyroscope)
- Glare effect 🌟 with custom props (color, position,...) 🔗demo
- Events to keep track of component values 📐 (tilt, glare, mousemove,...) 🔗demo
- Many effects that can be easily applied:
  - scale on hover 🔗demo
  - disable x/y axis 🔗demo
  - flip component vertically/horizontally 🔗demo
  - tilt hover effect on the whole window 🔗demo
  - tilt component with custom manual input 🕹 (joystick, slider etc.) 🔗demo
  - parallax effect on overlaid images 🔗demo

Example

    import React from 'react';
    import ReactDOM from 'react-dom';
    import Tilt from 'react-parallax-tilt';
    
    const App = () => {
      return (
        <Tilt>
          <div style={{ height: '300px', backgroundColor: 'darkgreen' }}>
            <h1>React Parallax Tilt 👀</h1>
          </div>
        </Tilt>
      );
    };
    
    ReactDOM.render(<App />, document.getElementById('root'));

Props

All of the props are optional.  

Below is the complete list of possible props and their options:

▶︎ indicates the default value if there's one

tiltEnable: boolean ▶︎ true  

Boolean to enable/disable tilt effect.

tiltReverse: boolean ▶︎ false  

Reverse the tilt direction.

tiltAngleXInitial: number ▶︎ 0  

Initial tilt value (degrees) on x axis.

tiltAngleYInitial: number ▶︎ 0  

Initial tilt value (degrees) on y axis.

tiltMaxAngleX: number ▶︎ 20  

Max tilt rotation (degrees) on x axis (range: 0°-90°).

tiltMaxAngleY: number ▶︎ 20  

Max tilt rotation (degrees) on y axis (range: 0°-90°).

tiltAxis: 'x' | 'y' ▶︎ undefined  

Enable tilt on single axis.

tiltAngleXManual: number | null} ▶︎ null  

Manual tilt rotation (degrees) on x axis.

tiltAngleYManual: number | null} ▶︎ null  

Manual tilt rotation (degrees) on y axis.

glareEnable: boolean ▶︎ false  

Boolean to enable/disable glare effect.

glareMaxOpacity: number ▶︎ 0.7  

The maximum glare opacity (range: 0-1).

glareColor: string ▶︎ #ffffff  

Set color of glare effect.

glareBorderRadius: string ▶︎ 0  

Accepts any standard CSS border radius. Useful if the glare color is different to the page color.

glarePosition: 'top' | 'right' | 'bottom' | 'left' | 'all' ▶︎ bottom  

Set position of glare effect.

glareReverse: boolean ▶︎ false  

Reverse the glare direction.

scale: number ▶︎ 1  

Scale of the component (1.5 = 150%, 2 = 200%, etc.).

perspective: number ▶︎ 1000  

The perspective property defines how far the object (wrapped/child component) is away from the user. The lower the more extreme the tilt gets.

flipVertically: boolean ▶︎ false  

Boolean to enable/disable vertical flip of component.

flipHorizontally: boolean ▶︎ false  

Boolean to enable/disable horizontal flip of component.

reset: boolean ▶︎ true  

If the effects has to be reset on onLeave event.

transitionEasing: string ▶︎ cubic-bezier(.03,.98,.52,.99)  

Easing of the transition when manipulating the component.

transitionSpeed: number ▶︎ 400  

Speed of the transition when manipulating the component.

trackOnWindow: boolean ▶︎ false  

Track mouse and touch events on the whole window.

gyroscope: boolean ▶︎ false  

Boolean to enable/disable device orientation detection.

onMove: Function => ({ tiltAngleX: number, tiltAngleY: number, tiltAngleXPercentage: number, tiltAngleYPercentage: number, glareAngle: number, glareOpacity: number, eventType: string }) => void  

Gets triggered when user moves on the component.

onEnter: Function => (eventType: string) => void  

Gets triggered when user enters the component.

onLeave: Function => (eventType: string) => void  

Gets triggered when user leaves the component.

Gyroscope - Device Orientation

Please keep in mind that detecting device orientation is currently experimental technology.  

Check the browser compatibility before using this in production.  

A few takeaways when using device orientation event:

- always use secure origins (such as https)
- it doesn't work in all browsers when using it in cross-origin <iframe> element

<details>

<summary>Using device orientation on iOS 13+</summary>

Apple decided turning device motion and orientation off by default since iOS 12.2.  

With iOS 13+ permission API can be used to gain access to device orientation event.

When using gyroscope feature:

    <Tilt gyroscope={true}>
      <h1>React Parallax Tilt 👀</h1>
    </Tilt>

it will present a permission dialog prompting the user to allow motion and orientation access at domain level:  



Note that user needs to take some action (like tapping a button) to be able to display the dialog (invoking dialog on page load is not possible).

</details>

Development

Easily set up a local development environment!

Build project and start storybook on localhost:

- clone
- npm install
- npm start

Start coding! 🎉

<details>

<summary>Or setup with npm link</summary>

Clone this repo on your machine, navigate to its location in the terminal and run:

    npm install
    npm link # link your local repo to your global packages
    npm run build:watch # build the files and watch for changes

Clone project repo that you wish to test with react-parallax-tilt library and run:

    npm install
    npm link react-parallax-tilt # link your local copy into this project's node_modules
    npm start

</details>

Contributing

All contributions are welcome!  

Please take a moment to review guidelines PR | Issues

[npm-url]: https://www.npmjs.com/package/react-parallax-tilt
[npm-badge]: https://img.shields.io/npm/v/react-parallax-tilt.svg
[size-badge]: https://badgen.net/bundlephobia/minzip/react-parallax-tilt
[downloads-badge]: https://img.shields.io/npm/dm/react-parallax-tilt.svg?color=blue
[lint-badge]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/lint.yml/badge.svg
[lint-url]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/lint.yml
[tsc-badge]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/tsc.yml/badge.svg
[tsc-url]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/tsc.yml
[build-badge]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/build.yml/badge.svg
[build-url]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/build.yml
[test-badge]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/test.yml/badge.svg
[test-url]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/test.yml
[deploy-storybook-badge]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/deploy-storybook.yml/badge.svg
[deploy-storybook-url]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/deploy-storybook.yml
[npm-release-badge]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/npm-release.yml/badge.svg
[npm-release-url]: https://github.com/mkosir/react-parallax-tilt/actions/workflows/npm-release.yml
[coverage-badge]: https://codecov.io/gh/mkosir/react-parallax-tilt/branch/main/graph/badge.svg
[coverage-url]: https://codecov.io/gh/mkosir/react-parallax-tilt
[issues-badge]: https://img.shields.io/github/issues/mkosir/react-parallax-tilt
[issues-url]: https://github.com/mkosir/react-parallax-tilt/issues
[semantic-badge]: https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg
[semantic-url]: https://github.com/semantic-release/semantic-release
[typescript-badge]: https://badges.frapsoft.com/typescript/code/typescript.svg?v=101
[typescript-url]: https://github.com/microsoft/TypeScript

---


