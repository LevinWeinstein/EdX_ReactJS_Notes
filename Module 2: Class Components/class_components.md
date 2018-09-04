# Class Components

## Class Components
In addition to being written as a function, React Components can also be written using ES6 classes. Class Components differ from Functional Components because they allow React Components to have **life cycle methods** and **state**. Class components have two instance properties, *this.state* and *this.props*, that represent the component's state and properties respectively.

#### React Component written using ES6 classes:
```jsx
class Welcome extends React.Component{
    render(){
        return <h1>Hello World!</h1>;
    }
}
```
This is the same as the following Functional Component:
```jsx
function Welcome(){
    return <h1>Hello World!</h1>;
}
```
Both types of React Components can be used by writing their name within an HTML tag:
```jsx
var element = <Welcome />
```

## Render()
The render() method of a class component is used to describe what kind of React Element is going to be returned from the Class Component. It is the same as the return value of a Functional Component.

For example, the following Class Component will render `<h1>Hello World!</h1>`:

```html
<div id="root"></div>
```

```jsx
class Welcome extends React.Component {
    render() {
        return <h1>Hello World!</h1>;
    }
}

//renders <h1>Hello World!</h1>
ReactDOM.render(
    <Welcome />,
    document.getElementById("root")
)
```

## Adding properties to Class Components
The properties of a Class Component can be accessed through the *this.props* attribute. This differs slightly from Functional Components where the properties were passed in as a veriable.

```jsx
class Welcome extends React.Component{
    render(){
        return <h1>Message: {this.props.message}</h1>;
    }
}
```
You can supply property values the same way as you supply attribute values:
```jsx
<Welcome message="Hello World!" />
```

