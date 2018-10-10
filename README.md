# jQuery Smart Cart 3
### The smart interactive jQuery Shopping Cart plugin with PayPal payment support.

jQuery Smart Cart is the smart interactive **jQuery Shopping Cart plugin** with **PayPal** payment support. It can create an interactive and user friendly shopping cart with minimal code. It has built-in support for **Form** submit, **Ajax** submit and **PayPal** submit of the cart items. A lot of customization options and custom events makes it easy to implement your requirements. It can integrate with your existing shopping list very easily and you can use your own css.

The new version **jQuery Smart Cart 3** is completely rewritten from scratch and adopted the modern patterns. It is more powerful, robust, scalable and customizable. A lot of features is added like Bootstrap support, theme support, customizable toolbars, customization options, public methods, event support and a lot more.
See the list of [features](http://techlaboratory.net/smartcart#features), [demos](http://techlaboratory.net/smartcart/demo) and [documentation](http://techlaboratory.net/smartcart/documentation) for more details.  

+ [Homepage](http://techlaboratory.net/smartcart)
+ [Documentation](http://techlaboratory.net/smartcart/documentation)
+ [Demos](http://techlaboratory.net/smartcart/demo)

Demos
-----
  + [Basic Example](http://techlaboratory.net/smartcart/demo/basic)
  + [PayPal Cart Example](http://techlaboratory.net/smartcart/demo/paypal)

Screenshots
-----
![Smart Cart Screenshot1](http://techlaboratory.net/assets/media/products/SmartCart3-Normal.png?v1)
![Smart Cart Screenshot2](http://techlaboratory.net/assets/media/products/SmartCart3-PayPal.png?v1)

Requirements
-----
  + [jQuery](http://jquery.com/) (supports jQuery 1.9+, jQuery 2+, jQuery 3+)

Installation and usage 
-----

### Bower
    bower install tete-chercheuse/smart-cart
    
### Download
#### [Download from GitHub](https://github.com/tete-chercheuse/smart-cart/archive/master.zip)    
###  
 Please see the [documentation](http://techlaboratory.net/smartcart/documentation) for more deatils on implementation and usage.

Features
-----
  + In-built PayPal, Ajax and form submit methods
  + Heavily customizable toolbar, option to add extra buttons
  + Theme support
  + Customizable css styles
  + Public methods for external function call
  + Enhanced event support
  + Compatible with latest jQuery versions (jQuery 1.9+, jQuery 2+, jQuery 3+)
  + Easy to implement, Minimal HTML required
  + Clean and compact design
  + Automatically calculates subtotal
  + Quantity is editable from the cart list
  + Product Image display
  + Customizable cart templates
  + Customizable currency formatting option
  + Pre-populate products on cart on load
  + and a lot more...
  
Options
-----
Here are all options with default values:

```javascript
var defaults = {
    cart:                     [], // initial products on cart
    resultName:               'cart_list', // Submit name of the cart parameter
    theme:                    'default', // theme for the cart, related css need to include for other than default theme
    combineProducts:          true, // combine similar products on cart
    highlightEffect:          true, // highlight effect on adding/updating product in cart
    cartItemTemplate:         '<td class="sc-cart-item-name"><h4>{product_name}</h4><p>{product_desc}</p></td><td class="sc-cart-item-price">{product_price}</td><td class="sc-cart-item-quantity">{product_quantity}</td><td class="sc-cart-item-amount">{product_total}</td>',
    cartHeaderTemplate:       '<th>Name</th><th>Price</th><th>Quantity</th><th>Total</th><th></th>',
    productContainerSelector: '.sc-product-item',
    productElementSelector:   '*', // input, textarea, select, div, p
    addCartSelector:          '.sc-add-to-cart',
    transitionsDuration:      300,
    quantityOptions:          {
        min:  0,
        max:  10,
        step: 5
    },
    paramSettings:            { // Map the paramters
        productPrice:    'product_price',
        productTotal:    'product_total',
        productQuantity: 'product_quantity',
        productName:     'product_name',
        productId:       'product_id'
    },
    lang:                     { // Language variables
        cartTitle:  "Shopping Cart",
        checkout:   'Checkout',
        clear:      'Clear',
        subtotal:   'Subtotal:',
        cartRemove: '×',
        cartEmpty:  'Cart is Empty'
    },
    submitSettings:           {
        submitType:   'form', // form, paypal, ajax
        ajaxURL:      '', // Ajax submit URL
        ajaxSettings: {} // Ajax extra settings for submit call
    },
    currencySettings:         {
        locales:         'en-US', // A string with a BCP 47 language tag, or an array of such strings
        currencyOptions: {
            style:           'currency',
            currency:        'USD',
            currencyDisplay: 'symbol' // extra settings for the currency formatter. Refer: https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Number/toLocaleString
        }
    },
    toolbarSettings:          {
        showToolbar:         true,
        showCheckoutButton:  true,
        showClearButton:     true,
        showCartSummary:     true,
        checkoutButtonStyle: 'default', // default, paypal, image
        checkoutButtonImage: '', // image for the checkout button
        toolbarExtraButtons: [] // Extra buttons to show on toolbar, array of jQuery input/buttons elements
    },
    debug:                    false
};
```
Version
-----
**smart-cart 3.0.2**

License
----
[MIT License](https://github.com/tete-chercheuse/smart-cart/blob/master/LICENSE)
