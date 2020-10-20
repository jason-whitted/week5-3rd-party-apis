# jQuery Selection

The `$` function can accept a string as a CSS selector to find zero or more more DOM elements.

```js
var myDiv = $("#my-div");
var thumbnails = $("img.thumbnails");
```

NOTE: In the API Documentation for jQuery, look up `Core > jQuery()` to find documentation for the signature of the `$` function.

## Signature
```js
(String) -> JQueryCollection
```

## The jQuery Collection
jQuery returns the elements in a collection of jQuery objects.  The resulting collection is array-like.  
It has a `length` property and you can access individual jQuery objects using an index.
```js
var divs = $("div");
var count = divs.length;
var first = divs[0];
```

## jQuery Objects vs jQuery Collections
In general:
- jQuery collections and jQuery objects share most of the same methods
  - NOTE: In the jQuery docs these methods are listed simply as the `jQuery API`
- when using a *getter* function from a jQuery collection it will read the value from the first object
- when using a *setter* function on a jQuery collection it will set the value on all objects in the collection
