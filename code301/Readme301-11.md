# Rest

Rest : is the HTTP method used to send request to our server standers.

|method|----|SQL|
|------|----|---|
|Get|READ|SELECT|
|Post|CREATE|INSERT|
|Put|UPDATE|UPDATE|
|Delete|DESTROY|DROP|

# How To Use EJS to Template Your Node Application

Jade comes as the view engine for Express by default but Jade syntax can be overly complex for many use cases. EJS is one alternative does that job well and is very easy to set up. Let’s take a look at how we can create a simple application and use EJS to include repeatable parts of our site (partials) and pass data to our views.

# Setting up the Demo App

1. File Structure

- views
----- partials
---------- footer.ejs
---------- head.ejs
---------- header.ejs
----- pages
---------- index.ejs
---------- about.ejs
- package.json
- server.js

2. Node Setup

npm install

// load the things we need
var express = require('express');
var app = express();

// set the view engine to ejs
app.set('view engine', 'ejs');

// use res.render to load up an ejs view file

// index page
app.get('/', function(req, res) {
    res.render('pages/index');
});

// about page
app.get('/about', function(req, res) {
    res.render('pages/about');
});

app.listen(8080);
console.log('8080 is the magic port');

node server.js

Create the EJS Partials

1. head.ejs

meta charset="UTF-8"
title EJS Is Fun /title

<!-- CSS (load bootstrap from a CDN) -->
link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.5.2/css/bootstrap.min.css"
style
    body { padding-top:50px; }
/style

2. header.ejs

nav class="navbar navbar-expand-lg navbar-light bg-light"
  a class="navbar-brand" href="/" EJS Is Fun /a
  ul class="navbar-nav mr-auto"
    li class="nav-item"
      a class="nav-link" href="/" Home /a
    /li
    li class="nav-item"
      a class="nav-link" href="/about" About /a
    /li
  /ul
/nav

3. footer

p class="text-center text-muted" © Copyright 2020 The Awesome People/p

# Add the EJS Partials to Views

Syntax for including an EJS Partial
Use <%- include('RELATIVE/PATH/TO/FILE') %> to embed an EJS partial in another file.

The hyphen <%- instead of just <% to tell EJS to render raw HTML.
The path to the partial is relative to the current file.

index.ejs

!DOCTYPE html
html lang="en"
head
    <%- include('../partials/head'); %>
/head
body class="container"

header
    <%- include('../partials/header'); %>
/header

main
    div class="jumbotron"
        h1 This is great /h1
        p Welcome to templating using EJS /p
    /div
/main

footer
    <%- include('../partials/footer'); %>
/footer

/body
/html