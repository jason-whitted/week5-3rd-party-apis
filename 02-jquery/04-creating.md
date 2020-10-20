# jQuery Element Creation
In jQuery you can create an element by simply writing the HTML.

```js
var myHeader = $('<header id="bob"><h1 class="fred">Hello World!</h1></header>');
// Just like document.createElement(),
// this code will not automatically attach it to the DOM.
// You will append or prepend the element via another method.
```

## Signature
```js
(String) -> jQueryObject
```
