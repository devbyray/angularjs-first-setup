# Angular Setup

## Project structure:
- app
    - src
        - js
            - libs
                - angular.min.js
            - app.js
        -sass
            - sass-structure
    - index.html
- gulpfile.js
- package.json
- readme.md

## How to install

1. run `(sudo) npm install`
2. run `gulp`
3. Then the browser will start.

## How to start an AngularJS app

In this example I already did the setup. But the most important things to do is:

1. Include the angular.js file & app.js file in the html (on the bottom of the page) `<script src="assets/js/libs/angular.min.js"></script><script src="assets/js/app.js"></script>`. But i prefer to concat all the .js files into 1 file. So that's why the index.html file only include app.js.
2. In the html replace the `<html>` with `<html ng-app>` to let Angular know that this is the Angular Root element.
3. Then in your html place the following expression: `1 + 2 = {{ 1 + 2 }}`. When AngularJS is loaded, it will do the math for you. [demo](http://codepen.io/rsschouwenaar/pen/QbWoRv)
4. In the app.js place this code to begin the application:
`var app = angular.module("app", []);`
