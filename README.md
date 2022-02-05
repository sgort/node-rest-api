# Doccle suite services demo

## API code base
Prototype code base for usage of a RESTful API with Node.js and Express Framework

- morgan is used for logging requests to the console
- nodemon is used for automatically restarting the server when your code changes

`npm start` is all you need after cloning the repo

```
steven@steven-Surface-Laptop-3:~/Development/node-rest-api$ npm start

> rest-api@1.0.0 start
> nodemon server.js

[nodemon] 2.0.15
[nodemon] to restart at any time, enter `rs`
[nodemon] watching path(s): *.*
[nodemon] watching extensions: js,mjs,json
[nodemon] starting `node server.js`
Connected to `DoccleTest`!
GET /products 200 37.649 ms - 723
{
  _id: new ObjectId("61fe49a37a72c91908feee8f"),
  name: 'Latest one POSTed',
  price: 2345,
  __v: 0
}
POST /products/ 201 57.984 ms - 223
GET /orders/61fe4606a0cebbde6e5237e7 200 31.595 ms - 165
{
  _id: new ObjectId("61fe4a057a72c91908feee93"),
  product: new ObjectId("61fe49a37a72c91908feee8f"),
  quantity: 666,
  __v: 0
}
POST /orders/ 201 64.962 ms - 215
```
## Postman collection
The Postman collection build for this demo is ![published here](https://documenter.getpostman.com/view/10824299/UVeGqkvR).