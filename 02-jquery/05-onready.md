# jQuery OnReady

## The Problem
Scripts are loaded syncronously.

```html
<html>
  <head>
    <script>
      document.querySelector("h1").textContent = "Hello World!";
    </script>
  </head>
  <body>
    <h1></h1>
  </body>
</html>
```

## One Solution
```html
<html>
  <head>
  </head>
  <body>
    <h1></h1>
    <script>
      document.querySelector("h1").textContent = "Hello World!";
    </script>
  </body>
</html>
```

## Another Solution
```html
<html>
  <head>
    <script>
      window.addEventListener("load", function() {
        document.querySelector("h1").textContent = "Hello World!";
      });
    </script>
  </head>
  <body>
    <h1></h1>
  </body>
</html>
```

## jQuery Solution
jQuery lets you pass a function to the `$` jQuery function and it will automatically bind it and run it when the document is ready.

```html
<html>
  <head>
    <script>
      $(function() {
        document.querySelector("h1").textContent = "Hello World!";
      });
    </script>
  </head>
  <body>
    <h1></h1>
  </body>
</html>
```
