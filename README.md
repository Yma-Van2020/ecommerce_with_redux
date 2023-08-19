# Codecademy Store

![An animated gif showing a demo of the Codecademy store's features](./shopping-cart-demo.gif)

This application has three slices of state:

- `inventory`: An array of objects representing the items that are available to purchase.

- `cart`: An object that maps the name of each item added to the cart to an object with the price and desired quantity for that item.
  
- `currencyFilter`: A string that represents the currency used to calculate the prices displayed to the user: 'USD', 'CAD' or 'EUR'.
  
An example of this application’s state might look like this:

```js
state = {
  inventory: [
    { name: 'Hat', img: 'img/hat.png', price: 15.99 },
    { name: 'T-Shirt', img: 'img/t-shirt.png', price: 18.99 },
    { name: 'Hoodie', img: 'img/hoodie.png', price: 49.99 },
  ],
  cart: {
    'Hat': { price: 15.99, quantity: 0 },
    'T-Shirt': { price: 15.99, quantity: 2 },
    'Hoodie': { price: 18.99, quantity: 1 },
  },
  currencyFilter: 'CAD'
}
```

As you will see, the file structure has been organized using the recommended feature-based pattern and most of the inventory and currency features have been built for you. It will be up to you to:

- complete the cart’s action creators and reducer logic

- create the store using createStore() and combineReducers()

- pass the store resources to presentational components via the top-level <App /> component

- render the <Cart /> component using the current state data

- dispatch actions to the store
