# The `ng-model` Directive

## Introduction

This directive tells AngularJS create a **data-binding** between the **View** and the
**Scope**. You apply it input elements, such as `<input>`, `<select>` and `<textarea>`, as an
attribute:

## Example

```html
<input type="text" ng-model="firstName">
```

## Explanation

- The value of the `ng-model` attribute is the property on the *scope* that is bound to what the user
has entered into the input.

Here we have an input field to enter your first name. Whatever you type into the input box is
assigned to a property on the a *scope* called `firstName`. Since `firstName` is a property on the
*scope*, you can in other parts of the view to display your first name. AngularJS keeps the scope
and the view in synch for you.