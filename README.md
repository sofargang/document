------

## CONTENTS OF THIS FILE

- Introduction
- Requirements
- Installation
- Configuration
- Maintainers

## INTRODUCTION

The Easy Breadcrumb module provides configurable breadcrumbs that improve oncore breadcrumbs by including the current page title as an unlinked crumb whichfollows breadcrumb best-practices(URL "<https://www.nngroup.com/articles/breadcrumb-navigation-useful/>").Easy Breadcrumb takes advantage of the work you've already done for generatingyour path aliases, while it naturally encourages the creation of semanticand consistent paths. This module is currently available for Drupal 6.x, 7.x,and 8.x.x.

Easy Breadcrumb uses the current URL (path alias) and the current page's titleto automatically extract the breadcrumb's segments and its respective links.The module is really a plug and play module because it auto-generates thebreadcrumb by using the current URL and nothing extra is needed.

- For the description of the module visit:<https://www.drupal.org/project/easy_breadcrumb>or<https://www.drupal.org/docs/8/improve-the-breadcrumbs>
- To submit bug reports and feature suggestions, or to track changes visit:<https://www.drupal.org/node/2929013>

## REQUIREMENTS

This module requires no modules outside of Drupal core.

## INSTALLATION

Install the Easy Breadcrumb module as you would normally install a contributedDrupal module. Visit <https://www.drupal.org/node/1897420> for furtherinformation.

## CONFIGURATION

```
1. Navigate to Administration > Extend and enable the module. The system
   breadcrumb block has now been updated.
2. Navigate to Administration > Configuration > User Interface > Easy
   Breadcrumb for configurations. Save Configurations.
```

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

## MAINTAINERS

- Greg Boggs - <https://www.drupal.org/u/greg-boggs>
- Neslee Canil Pinto - <https://www.drupal.org/u/neslee-canil-pinto>
- Brooke Mahoney (loopduplicate) - <https://www.drupal.org/u/loopduplicate>

Supporting organization:

- Kanopi Studios - <https://www.drupal.org/kanopi-studios>

------

# ![TOAST UI Editor](https://uicdn.toast.com/toastui/img/tui-editor-bi.png)

> GFM  Markdown and WYSIWYG Editor - Productive and Extensible

[![github release version](https://img.shields.io/github/v/release/nhn/tui.editor.svg?include_prereleases)](https://github.com/nhn/tui.editor/releases/latest) [![npm version](https://img.shields.io/npm/v/@toast-ui/editor.svg)](https://www.npmjs.com/package/@toast-ui/editor) [![license](https://img.shields.io/github/license/nhn/tui.editor.svg)](https://github.com/nhn/tui.editor/blob/master/LICENSE) [![PRs welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg)](https://github.com/nhn/tui.editor/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) [![code with hearth by NHN Cloud](https://img.shields.io/badge/%3C%2F%3E%20with%20%E2%99%A5%20by-NHN_Cloud-ff1414.svg)](https://github.com/nhn)

<img src="https://user-images.githubusercontent.com/37766175/121809054-446bac80-cc96-11eb-9139-08c6d9ad2d88.png" />

## 🚩 Table of Contents

- [Packages](#-packages)
- [Why TOAST UI Editor?](#-why-toast-ui-editor)
- [Features](#-features)
- [Examples](#-examples)
- [Browser Support](#-browser-support)
- [Pull Request Steps](#-pull-request-steps)
- [Contributing](#-contributing)
- [TOAST UI Family](#-toast-ui-family)
- [Used By](#-used-by)
- [License](#-license)

## 📦 Packages

### TOAST UI Editor

| Name                                     | Description                |
| ---------------------------------------- | -------------------------- |
| [`@toast-ui/editor`](https://github.com/nhn/tui.editor/tree/master/apps/editor) | Plain JavaScript component |

### TOAST UI Editor's Wrappers

| Name                                     | Description                              |
| ---------------------------------------- | ---------------------------------------- |
| [`@toast-ui/react-editor`](https://github.com/nhn/tui.editor/tree/master/apps/react-editor) | [React](https://reactjs.org/) wrapper component |
| [`@toast-ui/vue-editor`](https://github.com/nhn/tui.editor/tree/master/apps/vue-editor) | [Vue](https://vuejs.org/) wrapper component |

### TOAST UI Editor's Plugins

| Name                                     | Description                     |
| ---------------------------------------- | ------------------------------- |
| [`@toast-ui/editor-plugin-chart`](https://github.com/nhn/tui.editor/tree/master/plugins/chart) | Plugin to render chart          |
| [`@toast-ui/editor-plugin-code-syntax-highlight`](https://github.com/nhn/tui.editor/tree/master/plugins/code-syntax-highlight) | Plugin to highlight code syntax |
| [`@toast-ui/editor-plugin-color-syntax`](https://github.com/nhn/tui.editor/tree/master/plugins/color-syntax) | Plugin to color editing text    |
| [`@toast-ui/editor-plugin-table-merged-cell`](https://github.com/nhn/tui.editor/tree/master/plugins/table-merged-cell) | Plugin to merge table columns   |
| [`@toast-ui/editor-plugin-uml`](https://github.com/nhn/tui.editor/tree/master/plugins/uml) | Plugin to render UML            |

## 🤖 Why TOAST UI Editor?

TOAST UI Editor provides **Markdown mode** and **WYSIWYG mode**. Depending on the type of use you want like production of *Markdown* or maybe to just edit the *Markdown*. The TOAST UI Editor can be helpful for both the usage. It offers **Markdown mode** and **WYSIWYG mode**, which can be switched any point in time.

### Productive Markdown Mode

![markdown](https://user-images.githubusercontent.com/37766175/121464762-71e2fc80-c9ef-11eb-9a0a-7b06e08d3ccb.png)

**CommonMark + GFM Specifications**

Today *CommonMark* is the de-facto *Markdown* standard. *GFM (GitHub Flavored Markdown)* is another popular specification based on *CommonMark* - maintained by *GitHub*, which is the *Markdown* mostly used. TOAST UI Editor follows both [*CommonMark*](http://commonmark.org/) and [*GFM*](https://github.github.com/gfm/) specifications. Write documents with ease using productive tools provided by TOAST UI Editor and you can easily open the produced document wherever the specifications are supported.

- **Live Preview** : Edit Markdown while keeping an eye on the rendered HTML. Your edits will be applied immediately.
- **Scroll Sync** : Synchronous scrolling between Markdown and Preview. You don't need to scroll through each one separately.
- **Syntax Highlight** : You can check broken Markdown syntax immediately.

### Easy WYSIWYG Mode

![wysiwyg](https://user-images.githubusercontent.com/37766175/121808381-251f5000-cc93-11eb-8c47-4f5a809de2b3.png)

- **Table** : Through the context menu of the table, you can add or delete columns or rows of the table, and you can also arrange text in cells.
- **Custom Block Editor** : The custom block area can be edited through the internal editor.
- **Copy and Paste** : Paste anything from browser, screenshot, excel, powerpoint, etc.

### UI

- **Toolbar** : Through the toolbar, you can style or add elements to the document you are editing.
  ![UI](https://user-images.githubusercontent.com/37766175/121808231-767b0f80-cc92-11eb-82a0-433123746982.png)
- **Dark Theme** : You can use the dark theme.
  ![UI](https://user-images.githubusercontent.com/37766175/121808649-8136a400-cc94-11eb-8674-812e170ccab5.png)

### Use of Various Extended Functions - Plugins

![plugin](https://user-images.githubusercontent.com/37766175/121808323-d8d41000-cc92-11eb-9117-b92a435c9b43.png)

CommonMark and GFM are great, but we often need more abstraction. The TOAST UI Editor comes with powerful **Plugins** in compliance with the Markdown syntax.

**Five basic plugins** are provided as follows, and can be downloaded and used with npm.

- [**`chart`**](https://github.com/nhn/tui.editor/tree/master/plugins/chart) : A code block marked as a 'chart' will render [TOAST UI Chart](https://github.com/nhn/tui.chart).
- [**`code-syntax-highlight`**](https://github.com/nhn/tui.editor/tree/master/plugins/code-syntax-highlight) : Highlight the code block area corresponding to the language provided by [Prism.js](https://prismjs.com/).
- [**`color-syntax`**](https://github.com/nhn/tui.editor/tree/master/plugins/color-syntax) : 
  Using [TOAST UI ColorPicker](https://github.com/nhn/tui.color-picker), you can change the color of the editing text with the GUI.
- [**`table-merged-cell`**](https://github.com/nhn/tui.editor/tree/master/plugins/table-merged-cell) : 
  You can merge columns of the table header and body area.
- [**`uml`**](https://github.com/nhn/tui.editor/tree/master/plugins/uml) : A code block marked as an 'uml' will render [UML diagrams](http://plantuml.com/screenshot).

## 🎨 Features

- [Viewer](https://github.com/nhn/tui.editor/tree/master/docs/en/viewer.md) : Supports a mode to display only markdown data without an editing area.
- [Internationalization (i18n)](https://github.com/nhn/tui.editor/tree/master/docs/en/i18n.md) : Supports English, Dutch, Korean, Japanese, Chinese, Spanish, German, Russian, French, Ukrainian, Turkish, Finnish, Czech, Arabic, Polish, Galician, Swedish, Italian, Norwegian, Croatian + language and you can extend.
- [Widget](https://github.com/nhn/tui.editor/tree/master/docs/en/widget.md) : This feature allows you to configure the rules that replaces the string matching to a specific `RegExp` with the widget node.
- [Custom Block](https://github.com/nhn/tui.editor/tree/master/docs/en/custom-block.md) : Nodes not supported by Markdown can be defined through custom block. You can display the node what you want through writing the parsing logic with custom block.

## 🐾 Examples

- [Basic](https://nhn.github.io/tui.editor/latest/tutorial-example01-editor-basic)
- [Viewer](https://nhn.github.io/tui.editor/latest/tutorial-example04-viewer)
- [Using All Plugins](https://nhn.github.io/tui.editor/latest/tutorial-example12-editor-with-all-plugins)
- [Creating the User's Plugin](https://nhn.github.io/tui.editor/latest/tutorial-example13-creating-plugin)
- [Customizing the Toobar Buttons](https://nhn.github.io/tui.editor/latest/tutorial-example15-customizing-toolbar-buttons)
- [Internationalization (i18n)](https://nhn.github.io/tui.editor/latest/tutorial-example16-i18n)

Here are more [examples](https://nhn.github.io/tui.editor/latest/tutorial-example01-editor-basic) and play with TOAST UI Editor!

## 🌏 Browser Support

| <img src="https://user-images.githubusercontent.com/1215767/34348387-a2e64588-ea4d-11e7-8267-a43365103afe.png" alt="Chrome" width="16px" height="16px" /> Chrome | <img src="https://user-images.githubusercontent.com/1215767/34348590-250b3ca2-ea4f-11e7-9efb-da953359321f.png" alt="IE" width="16px" height="16px" /> Internet Explorer | <img src="https://user-images.githubusercontent.com/1215767/34348380-93e77ae8-ea4d-11e7-8696-9a989ddbbbf5.png" alt="Edge" width="16px" height="16px" /> Edge | <img src="https://user-images.githubusercontent.com/1215767/34348394-a981f892-ea4d-11e7-9156-d128d58386b9.png" alt="Safari" width="16px" height="16px" /> Safari | <img src="https://user-images.githubusercontent.com/1215767/34348383-9e7ed492-ea4d-11e7-910c-03b39d52f496.png" alt="Firefox" width="16px" height="16px" /> Firefox |
| :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: | :--------------------------------------: |
|                   Yes                    |                   11+                    |                   Yes                    |                   Yes                    |                   Yes                    |

## 🔧 Pull Request Steps

TOAST UI products are open source, so you can create a pull request(PR) after you fix issues. Run npm scripts and develop yourself with the following process.

### Setup

Fork `main` branch into your personal repository. Clone it to local computer. Install node modules. Before starting development, you should check if there are any errors.

```sh
$ git clone https://github.com/{your-personal-repo}/tui.editor.git
$ npm install
$ npm run build toastmark
$ npm run test editor
```

> TOAST UI Editor uses [npm workspace](https://docs.npmjs.com/cli/v7/using-npm/workspaces/), so you need to set the environment based on [npm7](https://github.blog/2021-02-02-npm-7-is-now-generally-available/). If subversion is used, dependencies must be installed by moving direct paths per package.

### Develop

You can see your code reflected as soon as you save the code by running a server. Don't miss adding test cases and then make green rights.

#### Run snowpack-dev-server

[snowpack](https://www.snowpack.dev/) allows you to run a development server without bundling.

```sh
$ npm run serve editor
```

#### Run webpack-dev-server

If testing of legacy browsers is required, the development server can still be run using a [webpack](https://webpack.js.org/).

```sh
$ npm run serve:ie editor
```

#### Run test

```sh
$ npm test editor
```

### Pull Request

Before uploading your PR, run test one last time to check if there are any errors. If it has no errors, commit and then push it!

For more information on PR's steps, please see links in the Contributing section.

## 💬 Contributing

- [Code of Conduct](https://github.com/nhn/tui.editor/blob/master/CODE_OF_CONDUCT.md)
- [Contributing Guideline](https://github.com/nhn/tui.editor/blob/master/CONTRIBUTING.md)
- [Commit Convention](https://github.com/nhn/tui.editor/blob/master/docs/COMMIT_MESSAGE_CONVENTION.md)
- [Issue Guidelines](https://github.com/nhn/tui.editor/tree/master/.github/ISSUE_TEMPLATE)

## 🍞 TOAST UI Family

- [TOAST UI Calendar](https://github.com/nhn/tui.calendar)
- [TOAST UI Chart](https://github.com/nhn/tui.chart)
- [TOAST UI Grid](https://github.com/nhn/tui.grid)
- [TOAST UI Image Editor](https://github.com/nhn/tui.image-editor)
- [TOAST UI Components](https://github.com/nhn)

## 🚀 Used By

- [NHN Dooray! - Collaboration Service (Project, Messenger, Mail, Calendar, Drive, Wiki, Contacts)](https://dooray.com)
- [UNOTES - Visual Studio Code Extension](https://marketplace.visualstudio.com/items?itemName=ryanmcalister.Unotes)

## 📜 License

This software is licensed under the [MIT](https://github.com/nhn/tui.editor/blob/master/LICENSE) © [NHN Cloud](https://github.com/nhn).

------

# React Tilt

[![npm version][npm-badge]][npm-url]
[![npm downloads][downloads-badge]][npm-url]
[![npm bundle size][size-badge]][npm-url]
[![Open issues][issues-badge]][issues-url]
[![TypeScript][typescript-badge]][typescript-url]
[![semantic-release][semantic-badge]][semantic-url]

[![CI][lint-badge]][lint-url]
[![CI][tsc-badge]][tsc-url]
[![CI][build-badge]][build-url]
[![CI][test-badge]][test-url]
[![Codecov Coverage][coverage-badge]][coverage-url]

[![CI][deploy-storybook-badge]][deploy-storybook-url]
[![CI][npm-release-badge]][npm-release-url]

_👀 Easily apply tilt hover effect on React components_

[![](misc/demo.gif)](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--glare-effect)

## [Demo 💥](https://mkosir.github.io/react-parallax-tilt)

## Install

```bash
npm install react-parallax-tilt
```

## Features

- Lightweight (≈3kB), zero dependencies 📦
- Works with React v15 onwards
- Supports **mouse** and **touch** events
- Support for device tilting (**gyroscope**)
- **Glare** effect 🌟 with custom props (color, position,...) [🔗demo](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--parallax-effect-glare-scale)
- Events to keep track of component values 📐 (tilt, glare, mousemove,...) [🔗demo](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--event-params)
- Many effects that can be easily applied:
  - **scale** on hover [🔗demo](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--scale)
  - **disable** x/y axis [🔗demo](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--tilt-disable-axis)
  - **flip** component vertically/horizontally [🔗demo](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--flip-vh)
  - tilt hover effect on the **whole window** [🔗demo](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--track-on-window)
  - tilt component with custom **manual input** 🕹 (joystick, slider etc.) [🔗demo](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--tilt-manual-input)
  - **parallax** effect on overlaid images [🔗demo](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--parallax-effect-img)

## Example

```jsx
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
```

## Props

All of the props are optional.  
Below is the complete list of possible props and their options:

> ▶︎ indicates the default value if there's one

**tiltEnable**: _boolean_ ▶︎ `true`  
Boolean to enable/disable tilt effect.

**tiltReverse**: _boolean_ ▶︎ `false`  
Reverse the tilt direction.

**tiltAngleXInitial**: _number_ ▶︎ `0`  
Initial tilt value (degrees) on x axis.

**tiltAngleYInitial**: _number_ ▶︎ `0`  
Initial tilt value (degrees) on y axis.

**tiltMaxAngleX**: _number_ ▶︎ `20`  
Max tilt rotation (degrees) on x axis (range: `0°-90°`).

**tiltMaxAngleY**: _number_ ▶︎ `20`  
Max tilt rotation (degrees) on y axis (range: `0°-90°`).

**tiltAxis**: _'x' | 'y'_ ▶︎ `undefined`  
Enable tilt on single axis.

**tiltAngleXManual**: _number_ | null} ▶︎ `null`  
Manual tilt rotation (degrees) on x axis.

**tiltAngleYManual**: _number_ | null} ▶︎ `null`  
Manual tilt rotation (degrees) on y axis.

**glareEnable**: _boolean_ ▶︎ `false`  
Boolean to enable/disable glare effect.

**glareMaxOpacity**: _number_ ▶︎ `0.7`  
The maximum glare opacity (range: `0-1`).

**glareColor**: _string_ ▶︎ `#ffffff`  
Set color of glare effect.

**glareBorderRadius**: _string_ ▶︎ `0`  
Accepts any standard CSS border radius. Useful if the glare color is different to the page color.

**glarePosition**: _'top' | 'right' | 'bottom' | 'left' | 'all'_ ▶︎ `bottom`  
Set position of glare effect.

**glareReverse**: _boolean_ ▶︎ `false`  
Reverse the glare direction.

**scale**: _number_ ▶︎ `1`  
Scale of the component (1.5 = 150%, 2 = 200%, etc.).

**perspective**: _number_ ▶︎ `1000`  
The perspective property defines how far the object (wrapped/child component) is away from the user. The lower the more extreme the tilt gets.

**flipVertically**: _boolean_ ▶︎ `false`  
Boolean to enable/disable vertical flip of component.

**flipHorizontally**: _boolean_ ▶︎ `false`  
Boolean to enable/disable horizontal flip of component.

**reset**: _boolean_ ▶︎ `true`  
If the effects has to be reset on `onLeave` event.

**transitionEasing**: _string_ ▶︎ `cubic-bezier(.03,.98,.52,.99)`  
Easing of the transition when manipulating the component.

**transitionSpeed**: _number_ ▶︎ `400`  
Speed of the transition when manipulating the component.

**trackOnWindow**: _boolean_ ▶︎ `false`  
Track mouse and touch events on the whole window.

**gyroscope**: _boolean_ ▶︎ `false`  
Boolean to enable/disable device orientation detection.

**onMove**: _Function_ => ({ **tiltAngleX**: _number_, **tiltAngleY**: _number_, **tiltAngleXPercentage**: _number_, **tiltAngleYPercentage**: _number_, **glareAngle**: _number_, **glareOpacity**: _number_, **eventType**: _string_ }) => _void_  
Gets triggered when user moves on the component.

**onEnter**: _Function_ => (**eventType**: _string_) => _void_  
Gets triggered when user enters the component.

**onLeave**: _Function_ => (**eventType**: _string_) => _void_  
Gets triggered when user leaves the component.

## Gyroscope - Device Orientation

Please keep in mind that detecting device orientation is currently [experimental technology](https://developer.mozilla.org/en-US/docs/MDN/Contribute/Guidelines/Conventions_definitions#Experimental).  
Check the [browser compatibility](https://caniuse.com/#search=DeviceOrientation) before using this in production.  
A few takeaways when using device orientation event:

- always use secure origins (such as `https`)
- it doesn't work in all browsers when using it in cross-origin `<iframe>` element

<details>
<summary>Using device orientation on iOS 13+</summary>

Apple decided turning device motion and orientation off by default since iOS 12.2.  
With iOS 13+ permission API can be used to gain access to device orientation event.

When using gyroscope feature:

```jsx
<Tilt gyroscope={true}>
  <h1>React Parallax Tilt 👀</h1>
</Tilt>
```

it will present a permission dialog prompting the user to allow motion and orientation access at domain level:  
![](misc/device_orientation.jpg)

Note that user needs to take some action (like tapping a button) to be able to display the dialog (invoking dialog on page load is not possible).

</details>

## Development

_Easily set up a local development environment!_

Build project and start storybook on [localhost](http://localhost:9009):

- clone
- `npm install`
- `npm start`

**Start coding!** 🎉

<details>
<summary>Or setup with npm link</summary>
Clone this repo on your machine, navigate to its location in the terminal and run:

```bash
npm install
npm link # link your local repo to your global packages
npm run build:watch # build the files and watch for changes
```

Clone project repo that you wish to test with react-parallax-tilt library and run:

```bash
npm install
npm link react-parallax-tilt # link your local copy into this project's node_modules
npm start
```

</details>

## Contributing

All contributions are welcome!  
Please take a moment to review guidelines [PR](.github/pull_request_template.md) | [Issues](https://github.com/mkosir/react-parallax-tilt/issues/new/choose)

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

------

