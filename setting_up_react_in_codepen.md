# The following steps are used to set up ReactJS to work in CodePen:

1. Go to https://codepen.io/pen to open a new project

2. Click Settings

3. Click JavaScript and under JavaScript Preprocessor select Babel

4. Click Quick-add and select React

5. Click Quick-add and select React-DOM (this must be selected after React or your app won't work)

## Once you have completed the above steps, add the following to get started:

* In HTML:
```html
<div id="root"></div>
```

* In JavaScript:
```javascript
ReactDOM.render(
    <div>HelloWorld</div>,
    document.getElementById("Root")
    )
