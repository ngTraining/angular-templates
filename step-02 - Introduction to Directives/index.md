#Introduction to Directives

##Declarative HTML

HTML is excellent at describing content for static documents in a declarative fashion.
For example if you wish to display an image of a map then you simply provide an `<img>` tag giving
it a `src` attribute telling the browser from where to get the image of the map:

```html
<img src="url/to/map.jpg"/>
```

The browser does the work of loading the image file and rendering it to the screen. Such is the
power of a declarative language.

But the HTML language is also limited. What if we wanted to display an **interactive map** that can
be **panned and zoomed**? Before HTML5 becomes mainstream, there is no `<map>` tag, which the
browser understands, to render interactive maps.

Traditionally, we would need to write a large amount of JavaScript to display such a dynamic map.
Moreover, there is no way to automatically display the map of an address that may be entered by the
user.

> What is needed is a way to teach the browser new HTML syntax.

## AngularJS Directives

**AngularJS** allows you to achieve functionality like this by using **directives** and
**data-binding**. It uses HTML as a template language, but lets us extend HTML's syntax to express
our application's visual components. In the case of maps, a developer could create am AngularJS
**map** directive that knows how to display maps. This directive could accept an `address`
attribute, which indicates what map to display:

```html
<map address="Buckingham Palace, London, UK"></map>
```

The HTML designer doesn't need to understand how the `<map>` directive works in order to use it.
Moreover the idea of a `<map>` tag fits in the world view of anyone who is used to working with
HTML. This is the power that AngularJS brings to building web applications.

AngularJS can add functionality to the browser by defining Directives that map to HTML elements,
attributes, classes and even comments. It has a set of directives built-in, which are useful for
building web applications. In addition we can define our own directives so that our HTML describes
our views in a way that is specific to our application domain.

In the next few sections we take a look at how to use some of the common AngularJS directives in our
applications.