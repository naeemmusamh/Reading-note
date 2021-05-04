# Classes

Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.

Classes are in fact "special functions", and just as you can define function expressions and function declarations, the class syntax has two components: class expressions and class declarations.

## Class declarations

class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
}

## Hoisting

Hoisting is a term you will not find used in any normative specification prose prior to ECMAScript® 2015 Language Specification.

const p = new Rectangle();

class Rectangle {}

## Class expressions

A class expression is another way to define a class. Class expressions can be named or unnamed. The name given to a named class expression is local to the class's body.


A- unnamed

let Rectangle = class {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
};
console.log(Rectangle.name);
// output: "Rectangle"


B- named

let Rectangle = class Rectangle2 {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
};
console.log(Rectangle.name);
// output: "Rectangle2"


## Class body and method definitions

1. Strict mode

code written here is subject to stricter syntax for increased performance

2. Constructor

a special method for creating and initializing an object created with a class.

3. Prototype methods

class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
  // Getter
  get area() {
    return this.calcArea();
  }
  // Method
  calcArea() {
    return this.height * this.width;
  }
}

const square = new Rectangle(10, 10);

console.log(square.area); // 100

# Routing

Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing.

You define routing using methods of the Express app object that correspond to HTTP methods:

var express = require('express')
var app = express()

to handle GET requests and app :

app.get('/', function (req, res) {
  res.send('hello world')
})

## Route methods

A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.

1. routes that are defined for the GET :

app.get('/', function (req, res) {
  res.send('GET request to the homepage');
});

2. routes that are defined for the POST :

app.post('/', function (req, res) {
  res.send('POST request to the homepage');
});

3. There is a special routing method, app.all(), used to load middleware functions at a path for all HTTP request methods.

app.all('/secret', function (req, res, next) {
  console.log('Accessing the secret section ...');
  next();
});

## Route Paths

Route paths, in combination with a request method, define the endpoints at which requests can be made, Route paths can be strings.

|Route Paths|Request to route|
|-----|-----|
|/|to the root route, /|
|/about|to /about.|
|/random.text|to /random.text|
|/ab?cd|match acd and abcd.|
|/ab+cd|match abcd, abbcd, abbbcd|
|/ab*cd|match abcd, abxcd, abRANDOMcd, ab123cd|
|/ab(cd)?e|match /abe and /abcde|
|/a/|match anything with an “a” in it.|
|/.*fly$/|match butterfly and dragonfly, but not butterflyman, dragonflyman|
|||

## Route parameters

Route parameters are named URL segments that are used to capture the values specified at their position in the URL.

Route path: /users/:userId/books/:bookId
Request URL: http://localhost:3000/users/34/books/8989
req.params: { "userId": "34", "bookId": "8989" }


app.get('/users/:userId/books/:bookId', function (req, res) {
  res.send(req.params)
})

