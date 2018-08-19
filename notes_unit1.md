# Setting up ReactJS

## The following steps are used to add ReactJS to an HTML file:

1. Create an HTML file

```html

<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
    </head>
    <body>
    </body>
</html>
```
2. Add scripts to include react.js, react-dom.js and babel.js inside the head of the HTML file

```html
<!DOCTYPE html>
<html>
  <head>
       <meta charset="UTF-8">
       <script src="https://unpkg.com/react@15/dist/react.min.js"></script>
       <script src="https://unpkg.com/react-dom@15/dist/react-dom.min.js"></script>
       <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/6.24.0/babel.js"></script>

  </head>
  <body>
  
  </body>
</html>
```

3. Add a babel script within the body of the HTML file.

```html
<!DOCTYPE html>
<html>
  <head>
       <meta charset="UTF-8">
       <script src="https://unpkg.com/react@15/dist/react.min.js"></script>
       <script src="https://unpkg.com/react-dom@15/dist/react-dom.min.js"></script>
       <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/6.24.0/babel.js"></script>

  </head>
  <body>

    <script type="text/babel">
  
    </script>

  </body>
</html>
```
4. Add `<div id="root"></div>` to the body of the HTML file
```html
<!DOCTYPE html>
<html>
  <head>
       <meta charset="UTF-8">
       <script src="https://unpkg.com/react@15/dist/react.min.js"></script>
       <script src="https://unpkg.com/react-dom@15/dist/react-dom.min.js"></script>
       <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/6.24.0/babel.js"></script>

  </head>
  <body>
    
    <div id="root"></div>
    <script type="text/babel">
  
    </script>

  </body>
</html>
```

5. Start rendering elements using ReactJS

```html
<!DOCTYPE html>
<html>
  <head>
       <meta charset="UTF-8">
       <script src="https://unpkg.com/react@15/dist/react.min.js"></script>
       <script src="https://unpkg.com/react-dom@15/dist/react-dom.min.js"></script>
       <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/6.24.0/babel.js"></script>

  </head>
  <body>
    
    <div id="root"></div>
    <script type="text/babel">
        ReactDOM.render(
            <div>Hello World</div>,
            document.getElementById("root")
            )
    </script>

  </body>
</html>
```

