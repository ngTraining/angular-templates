#Step 3 - The `ng-app` Directive

##Overview

This directive defines your application.  You place it as an attribute on an HTML element.  This
tells AngularJS that this element and all of its children are part of an AngularJS application.
**There can only be one `ng-app` per page**. We usually place it near the root of the page, for
example as
```
<html ng-app>
```
or 
```
<body ng-app>
```

##Example

In this example we create our first simple AngularJS application.

```html
<!doctype html>
<html ng-app>
  <body>
     <p>1 + 2 = {{ 1 + 2 }}</p>
     
     <script src="http://code.angularjs.org/1.2.0-rc.2/angular.min.js"></script>
  </body>

</html>
```
Here is a [link to the example](example-01).

## Explanation
* Loaded the `angular.js` file using the `<script>` tag at the bottom of the `<body>` tag.
* Applied the `ng-app` directive to the `<html>` tag so that the entire page is an AngularJS
  application.
* Bound an **interpolation expression** `{{ 1 + 2 }}` to the view

AngularJS has a special data-binding syntax called **interpolation**.  The bit of text in curly
braces `{{}}` is recognised by AngularJS as an **expression**, which will be evaluated against the
**scope**. The result is that the browser renders `1 + 2 = 3`.

If we did not specify an AngularJS application with `ng-app` then AngularJS would not interpret this
text and the browser would have rendered `1 + 2 = {{ 1 + 2 }}`.