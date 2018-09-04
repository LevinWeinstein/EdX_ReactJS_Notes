# Conditional Rendering

## Conditional Rendering
The output of a Functional Component can be determined based on its properties.

For example:
```jsx
function Feature(props){
    if (props.active == true){
        return <h1>This feature is active</h1>
    }
    else{
        return <h1>This feature is not active</h1>
    }
}
```
This can also be accomplished using an inline conditional operator:
```jsx
function Feature(props){
    return <h1>This feature is {props.active ? "active" : "not active"}</h1>
}
```

## Preventing Rendering
The output of a Functional Component can be prevented from rendering.

For example:
```jsx
function Feature(props){
    if (!props.active){
        return null;
    }
    else{
        return <h1>{props.message}</h1>
    }
}
```
You can also conditionally prevent a feature from rendering using the && operator:
```jsx
function Feature(props){
    return (
    props.active && <h1>{props.message}</h1>
    )
}
```
With the && operator, __true__ and __expression__ will always evaluate to __expression__. On the other hand, __false__ and __expression__ will always evaluate to false which won't render.
