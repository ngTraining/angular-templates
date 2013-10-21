# Step 1 - Loading AngularJS

##Overview
Before we can use AngularJS to create an application, we need to load it into the browser.

##Example

```html
<script src="../../lib/angular.js"></script>
```

##Explanation

We load AngularJS using a `<script>` element.

* The `<script>` tag tells the browser to download and run the `angular.js` JavaScript file.
* We are using a **relative URL** to point to a file stored locally in the `../../lib` folder.

>You can download the `angular.js` file from http://code.angularjs.org/.

Once the script is loaded we are ready to make our app.  We do this by adding **directives** to the
HTML.


We normally place this `<script>` tag in the `<head>` tag or at the bottom of the `<body>` tag. Once
the script is loaded we are ready to make our application. We do this by adding directives to the
HTML.