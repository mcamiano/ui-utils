# AngularUI - The companion suite for AngularJS

***

[![Build Status](https://travis-ci.org/angular-ui/ui-utils.png?branch=master)](https://travis-ci.org/angular-ui/ui-utils)

## Usage

### Requirements

* **AngularJS v1.0.0+** is currently required.
* **jQuery*** Until the refactor is complete, some directives still require jQuery

## Installation

Add the specific modules to your dependencies, or add the entire lib by depending on `ui.utils`

```javascript
angular.module('myApp', ['ui.keypress', 'ui.event', ...])
// or if ALL modules are loaded along with modules/utils.js
angular.module('myApp', ['ui.utils'])
```

Each directive and filter is now it's own module and will have a relevant README.md in their respective folders

### Requirements

0. Install [Node.js](http://nodejs.org/) and NPM (should come with)
   If you already have Node.js and NPM, make sure they are up to date.

1. Install global dependencies `grunt-cli`, `bower`, and `karma`:

    ```bash
    $ npm install -g karma grunt-cli bower
    ```

2. Install local dependencies:

    ```bash
    $ npm install
    $ bower install
    ```

Make sure the grunt packages are installed: 

```bash
$ npm install grunt-contrib-uglify
$ npm install grunt-contrib-watch
$ npm install grunt-contrib-concat
$ npm install grunt-contrib-clean
$ npm install grunt-contrib-jshint
$ npm install grunt-contrib-copy
$ npm install grunt-karma
$ npm install grunt
```

### Building


A "gruntFile.js" is available for building a combined script of all the modules in components/angular-ui-docs/build/ui-utils.js
Minified and versions with IEShiv are also included. 

_The myfork.master branch in this repo has been hacked to symlink ./dist to components/angular-ui-docs/build._

### Running Tests

Make sure all tests pass in order for your Pull Request to be accepted

You can choose what browsers to test in: `Chrome,ChromeCanary,Firefox,PhantomJS`

```bash
$ karma start --browsers=Chrome,Firefox test/karma.conf.js --single-run=true
```
