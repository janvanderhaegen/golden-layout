# [Golden Layout](https://golden-layout.com/)  [![NPM version](https://badge.fury.io/js/golden-layout.svg)](http://badge.fury.io/js/golden-layout) [![Build Status](https://travis-ci.org/deepstreamIO/golden-layout.svg?branch=master)](https://travis-ci.org/deepstreamIO/golden-layout)

![Screenshot](https://cloud.githubusercontent.com/assets/512416/4584449/e6c154a0-4ffa-11e4-81a8-a7e5f8689dc5.PNG)

# [https://golden-layout.com/](https://golden-layout.com/)
This is a branch taken from 1.5.9 (before the 2.0 rewrite in TS using modern module loaders).

Our project requires that some panels have an optional visiblity. AKA, they should only be visible if some conditions are met, for example show a detail panel only if a record is selected in the main panel.  We couldn't implement this using existing functionality like adding/removing panels, because we serialize the layout and restore it on refresh. Having a panel not visible because of business logic isn't the same as the user closing that panel.

Also, upgrading to the modern 2.0 version of this library would be too much work and have too many impacts due to our project not supporting modern module loaders.  We're not maintaining this or have plans for additional expansions.

Note: the API methods added are called "remember" and "forget", to make sure we have no name clashes with existing (internal) methods "show" and "hide".


## Installation

Add `golden-layout` to your bower.json, or [download](https://golden-layout.com/download/) the source.

## Features

* Native popup windows
* Completely themeable
* Comprehensive API
* Powerful persistence
* Works in IE8+, Firefox, Chrome
* Reponsive design


## [Examples](https://golden-layout.com/examples/)

## License
MIT

## Make it work
Press F5
The browser uses the individual files (LayoutManager.js, Root.js etc). Press CTRL+F5 to refresh and pick up changes.

Gulp/npm is broken due to old dependencies. Make changes to goldenlayout.js manually.

Original steps below:


### Prerequisites
Requires node 10. Use nvm (or nvm for windows)
$ cd /to/your/project/
$ nvm install 10
$ nvm use 10.0.0
$ npm install

### Run
$ cd /to/your/project/
$ gulp build (or gulp dev)
