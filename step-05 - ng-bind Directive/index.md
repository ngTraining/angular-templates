#Step 5 - The `ng-bind` Directive

##Overview
The `ng-bind` directive binds the text content of an element to the value of an **AngularJS
expression**. It is applied as an attribute to the element. The value of the attribute is the
**expression** to bind.

- Whenever the value of the expression changes, AngularJS will update
  the text content of the element with the new value.

##Example
This example shows the `ng-model` and `ng-bind` directives working together to display what the
user types.

```html
  Enter your first name: <input type="text" ng-model="firstName"><br/>
  <p>Hello <span ng-bind="firstName">!</p>
```

Here is a [link to the example](example).

###What's Going On Here?

- The `<input>` is bound to the `firstName` property on the scope.
- The `<span>` is also bound to the `firstName` property.
- When the user types in the `<input>` the text in the `<span>` is updated accordingly.

##Task

Extend the example with extra fields for **last name** and **description**.

* Use `ng-model` to bind an `<input>` field to insert your last name.
* Use `ng-model` to bind a `<textarea>` field to insert an interesting thing about you.
* Use `ng-bind` to display the information that you inserted in a separate `<p>` section.

Here is a link to a [starting point](task) for the task.