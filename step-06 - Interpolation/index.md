#Step 6 - Interpolation

##Overview

As well as the `ng-bind` directive, AngularJS provides a shorter notation for data binding.  This is
known as **interpolation**. You create an **interpolation binding** by wrapping an **AngularJS
expression** in double curly brackets, `{{...}}`.

Whenever the value of the expression changes, AngularJS will convert it to a string and replace the
**interpolation binding** with this string.

> Rather than a one-time insert, the **interpolation binding** dynamically updates whenever the
value of the **expression** changes.

One thing that interpolation can do, which `ng-bind` cannot is bind expressions to HTML attributes.
Because of this and its simpler syntax, you will mostly use the `{{ }}` syntax instead of the
`ng-bind` directive.

##Example

This example demonstrates the use of **interpolation**, both **in the text** and also **in an
attribute**.

```html
Your name: <input type="text" ng-model="name"/>
Your favourite colour: <input type="text" ng-model="colour"/>

<p>Hello {{name}}! I see that you like <span style="color: {{colour}}">{{colour}}</span></p>
```

Here is a [link to the example](example).

##Explanation
* The `<input>` elements are bound, by `ng-model`, to the `name` and `colour` properties on the
  **scope**.
* The text in the `<p>` element contains **interpolation bindings** to these properties.
* The `style` attribute has an **interpolation binding** to the `colour` property.
* If you type a colour, such as "red" or "blue", in the second `<input>` the text in the `<span>`
  will change to that colour.

##Task
Extend the example by creating a link to send an **email** to yourself.

* Use `ng-model` to bind an `<input>` field to insert your email.
* Use **interpolation** to create a `<a>` to click to send emails.

Here is a link to a [starting point](task) for the task.

##Homework

##References

