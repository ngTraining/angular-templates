#Interpolation

##Overview
This is the core feature of Angular's templating capabilities – a binding, denoted by **double-curlies {{ }}**.
The binding tells Angular that it should evaluate the expression inside the double-curlies and insert the result into the DOM in the place of the binding. Rather than a one-time insert, a binding will result in efficient continuous updates whenever the result of the expression evaluation changes. More often than not you will use the {{ }} syntax instead of the ng-bind directive.

##Example
```html
<label>Your name:</label>
<input type="text" ng-model="name"/>
<label>Your favourite colour: </label>
<input type="text" ng-model="colour"/>
<p>Hello {{name}}! I see that you like <span style="color: {{colour}}"> {{colour}}</span></p>
```

Here is a [link to the example](example).

##Explanation
* We have created two `input` boxes
* Using `ng-model` we bound the name and colour variable to the model
* After the template is processed by Angular, the name and colour variables in the double-curlies
are replaced by the values that you typed in the `input` boxes.

>Double-curlie bindings are not only used as the text of html elements. They can be used in html attributes and classes as well.

##Task
Extend the example by creating a link to send an **email** to yourself.

* Use `ng-model` to bind an `<input>` field to insert your email.
* Use double curlies to create a `<a>` to click to send emails.

Here is a link to a [starting point](task) for the task.

##Homework

##References

