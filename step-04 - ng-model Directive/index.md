#Step 4 - The `ng-model` Directive

## Introduction

This **directive** tells AngularJS to create a **data-binding** between the **View** and the
**Scope**. You apply it to input elements, such as `<input>`, `<select>` and `<textarea>`, as an
attribute. The value of the attribute is the **AngularJS expression** to bind.

AngularJS will keep the value of the expression and the value of the input element synchronized.

## Example
Here we bind a text input element to the `firstName` property on the **scope**.

```html
Enter your first name: <input type="text" ng-model="firstName"><br/>
Hello {{ firstName }}!
```

## Explanation

- The value of the `ng-model` attribute maps to the `firstName` property on the *scope*.
- When you type into the input box, AngularJS automatically updates the value of `firstName` on the
  scope
- The `{{firstName}}` **interpolation** displays this value as it changes.

Here we have an input field to enter your first name. Whatever you type into the input box is
assigned to a property on the a *scope* called `firstName`. Since `firstName` is a property on the
*scope*, you can bind to it in other parts of the view to display your first name. AngularJS keeps
the scope and the view in synch for you.
