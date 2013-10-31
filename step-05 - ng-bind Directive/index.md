#Step 5 - The `ng-bind` Directive and Interpolation

##ng-bind
The `ng-bind` directive binds the text content of an element to the value of an **AngularJS
expression**. It is applied as an attribute to the element. The value of the attribute is the
**expression** to bind.

- Whenever the value of the expression changes, AngularJS will update
  the text content of the element with the new value.

##Example
Modifying the example given for `ng-model`, we can display the name entered using `ng-bind`:

```html
<!doctype html>
<html ng-app>
  <body>
     <label>Your first name:</label>
     <input type="text" ng-model="firstName"/>
     <p>Hello <span ng-bind="firstName"></p>
     <script src="http://code.angularjs.org/1.2.0-rc.2/angular.min.js"></script>
  </body>
</html>
```

Here is a [link to the example](example).

##Explanation

This example shows the `ng-model` and `ng-bind` directives working together to display what the
user types.

##Task

Extend the example with extra fields for **last name** and **description**.

* Use `ng-model` to bind an `<input>` field to insert your last name.
* Use `ng-model` to bind a `<textarea>` field to insert an interesting thing about you.
* Use `ng-bind` to display the information that you inserted in a separate `<p>` section.

Here is a link to a [starting point](task-start) for the task.