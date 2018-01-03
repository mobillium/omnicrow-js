# Omnicrow Javascript SDK


To use **Omnicrow Javascript SDK**, you have to communicate with us through [Mobillium](http://www.mobillium.com)

## Installation

In the Browser
To use the SDK in the browser, simply add the following script tag to your HTML pages:

```html
<script type="text/javascript" src="https://dev.tubitak.mobillium.com/sdk.js"></script>
```

## Usage

### Initialize

```js
Omnicrow.init(baseUrl);

```

### Login

```js
Omnicrow.login(userId);
```


## Events
### Product Views

```js
Omnicrow.item(itemId);

```

### Category Views

Examples: ***"Category"*** ,  ***"Category > Subcategory"***

```js
Omnicrow.category(categoryPath);
```

### Add to Cart Events

```js
Omnicrow.cart([
    {
        id: itemId,
        quantity: itemQuantity,
        price: itemPrice,
    },
    {
        id: itemId,
        quantity: itemQuantity,
        price: itemPrice,
    },
    ...
]);

```

### Purchase Events

```js
Omnicrow.purchase(orderId, totalAmount, [
    {
        id: itemId,
        quantity: itemQuantity,
        price: itemPrice,
    },
    {
        id: itemId,
        quantity: itemQuantity,
        price: itemPrice,
    },
    ...
]);

```

## License

Omnicrow is available under the MIT license. See the LICENSE file for more info.

