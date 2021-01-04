# OBJECT-ORIENTED PROGRAMMING
## KEEPING UP WITH THE JAVASCRIPTS: ES6
## Homework 12: Object Oriented Programming
### theogn97, 2021

Object oriented programming is a programming/coding paradigm heavily based on objects. Real world things are represented as objects with key-value pairs as the objects' properties. These objects also have procedures and functions to allow data manipulation. OOP is used to structure data into simple and reusable pieces of code blueprints, usually called classes, which are used to create instances of objects. Object oriented programming is very useful to create complex applications because object oriented programming simplifies code into classes and object instances.

An application which will most likely benefit from object oriented programming is an e-commerce app. This e-commerce application allows people to sign up as users, providing a name (first and last names), username, email, address and password. Users can also update their personal information, such as username and/or password. Online store owners may upload listings of their products, providing a name, a description, photos, price, items in stock, and the minimum amount it takes for consumers to buy the product. These information can also be updated later. Consumers can add products into their wishlist or shopping cart and then make a checkout when they are sure to purchase. Then the users are led into the payment process where they complete the purchase. Stores can keep track of incoming orders and manage them. Users can also review a product using a 5-star rating and a review description, as well as chat with the store owners/managers.

CRUD operations performed by users include the following:
- Create and update a user profile
- Read lists of products available, as well as search for products
- Create and update product listings
- Add products into a user's wishlist or shopping cart
- Completion of payment
- Write a review of the product
- Chat (create messages) between users

Main objects of the system include:  
User object (constructor)  
`function User (id, firstName, lastName, username, address, email, password) {`  
`    this.id = id;`  
`    this.firstName = firstName;`  
`    this.lastName = lastName;`  
`    this.username = username;`  
`    this.address = address;`  
`    this.email = email;`  
`    this.password = password;`  
`}`  
Product object (constructor)  
`function Product(id, user, name, description, photoArray, timestamp, price, stock, minimumOrder) {`  
`    this.id = id;`  
`    this.user = user;`  
`    this.name = name;`  
`    this.description = description;`  
`    this.photoArray = photoArray; // photoArray is an array of picture data`  
`    this.timestamp = timestamp;`  
`    this.price = price;`  
`    this.stock = stock;`  
`    this.minimumOrder = minimumOrder;`  
`}`  
Wishlist object (constructor)  
`function Wishlist(user, wishlistArray) {`  
`    this.user = user;`  
`    this.wishlistArray = this.wishlistArray; // wishlistArray is an array of product IDs`  
`}`  
Cart object (constructor)  
`function Cart(user, cartArray) {`  
`    this.user = user;`  
`    this.cartArray = cartArray; // cartArray is an array of objects each containing a product ID and amount of purchase for that product`  
`}`  
Order object (constructor)  
`function Order(user, productID, amount, status) {`  
`    this.user = user;`  
`    this.productID = productID;`  
`    this.amount = amount;`  
`    this.status = status; // Status defines the status of the product delivery from the online store`  
`}`  
Chat object (constructor)  
`function Chat(sender, recipient, timestamp, message) {`  
`    this.sender = sender;`  
`    this.recipient = recipient;`  
`    this.timestamp = timestamp;`  
`    this.message = message;`  
`}`  

All of the above objects are related together on the user ID, and some of them are related on the product ID
