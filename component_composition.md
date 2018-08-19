# Composition

## Composing Components
Functional Components can include other Functional Components in their output. This lets us keep our components organized and readable.

For example, look at this Shopping Application that makes use of Composition:
```jsx
function ShoppingTitle(props){
    return (
        <div>
            <h1>{props.title}</h1>
            <h2>Total Number of Items: {props.numItems}</h2>
        </div>
    )
}

function ListItem(props){
    return <li>{props.item}</li>
}

function ShoppingList(props){
    return (
    <div>
        <h3>{props.header}</h3>
        <ol>
            <ListItem item = {props.items[0]}/>
            <ListItem item = {props.items[1]}/>
            <ListItem item = {props.items[2]}/>
        </ol>
    </div>
    )
}

function ShoppingApp(props){
    return (
        <div>
            <ShoppingTitle title="My Shopping List" numItems="9"/>
            <ShoppingList header="Food" items={["Apple", "Bread", "Cheese"]}/>
            <ShoppingList header="Clothes" item={["Shirt", "Pants", "Hat"]}/>
            <ShoppingList header="Supplies" items={["Pen","Paper","Glue"]}/>
        </div>
    )
}

ReactDOM.render(
    <ShoppingApp/>,
    document.getElementById("root")
)
```
Comparse that to just defining all the UI in one Functional Component
```jsx

    function ShoppingApp(props){
        return (
            <div>
                <div>
                    <h1>My Shopping List</h1>
                    <h2>Total Number of Items: 9</h2>
                </div>
                <div>
                    <h3>Food</h3>
                    <ol>
                        <li>Apple</li>
                        <li>Bread</li>
                        <li>Cheese</li>
                    </ol>
                </div>

                <div>
                    <h3>Clothes</h3>
                    <ol>
                        <li>Shirt</li>
                        <li>Pants</li>
                        <li>Hat</li>
                    </ol>
                </div>

                <div>
                    <h3>Supplies</h3>
                    <ol>
                        <li>Pen</li>
                        <li>Paper</li>
                        <li>Glue</li>
                    </ol>
                </div>


            </div>
        )
    }

    ReactDOM.render(
        <ShoppingApp/>,
        document.getElementById("root")
    )
```
