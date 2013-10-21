#Step 3 - The `ng-app` Directive

##Overview

This **directive** defines your AngularJS application.  You place it as an **attribute** on an HTML
element.  It tells AngularJS that this element and all of its children are part of an **AngularJS
application**.

We usually place this directive near the root element of the page, for example as `<html ng-app>` or
`<body ng-app>`.

>There can only be one `ng-app` per page.

##Example

In this example we create our first, simple AngularJS application.

```html
<!doctype html>
<html ng-app>
  <head>
    <script src="http://code.angularjs.org/1.2.0-rc.2/angular.min.js"></script>
  </head>
  <body>
     <p>1 + 2 = {{ 1 + 2 }}</p>
  </body>
</html>
```
Here is a [link to the example](example-01).

## Explanation

	This example demonstrates the basic elements that are needed to get an AngularJS application
running.

* Load the `angular.js` file using the `<script>` in the `<head>` tag.
* Apply the `ng-app` directive to the `<html>` tag so that the entire page is an **AngularJS
  application**.
* Bind an **interpolation expression** `{{ 1 + 2 }}` to the view

If we did not specify an AngularJS application with `ng-app` then AngularJS would not interpret this
text and the browser would have rendered `1 + 2 = {{ 1 + 2 }}`.

> AngularJS has a special data-binding syntax called **interpolation**. The bit of text in curly
> braces `{{}}` is recognised by AngularJS as an **expression**, which will be evaluated against the
> **scope**. The result is that the browser renders `1 + 2 = 3`.
>
> **This is covered, in detail, in later steps.**
