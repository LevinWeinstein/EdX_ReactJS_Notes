# What is ReactJS?


## What is ReactJS?
* ReactJS is a library that generates the view layer of an application based on its state. ReactJS applications are built from React Components - independent reusable components that describe how the UI should look based on their own state and properties.

## Why should I use ReactJS?
* ReactJS applications are incredibly performant at UI rerendering.
* React Components make writing UI components easier.

## What makes ReactJS so efficient at rerendering?
* React Components are ued to generate a Virtual DOM - a light-weight abstraction of the actual HTML DOM. The Virtual DOM is able to be generated much more quickly than the HTML DOM because it does not have to calculate the CSS styles and layouts. When a React Component changes state, the Virtual DOM is recreated and the difference between the new Virtual DOM and the previous Virtual DOM is calculated. The ReactJS library then calculates the most efficient way to update the HTML DOM to reflect these changes. This ends up being much faster than regenerating the entire HTML DOM from the top.

## How hard is it to use ReactJS?
* ReactJS is a relatively lightweight library and it does not take a whole lot of code to get started with it.

* Here is an ecample of the code needed for a Hello World application:
```html
<div id="root"></div>
```

```javascript
ReactDOM.render(
    <h1>Hello World!</h1>,
    document.getElemenetById("root")
    )
```
