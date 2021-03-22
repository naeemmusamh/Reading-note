# MUSTACHE and FLEXBOX

# Javascript Templating

Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source.
The template is HTML markup, with added templating tags that will either insert variables or run programming logic.

# Mustache

Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.

It is often referred to as “logic-less” because there are no if statements, else clauses, or for loops. Instead, there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.

mustache.js is an implementation of the mustache template system in JavaScript. It is often considered the base for JavaScript templating.

Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });
// returns: Hello, Sherlynn

A confusion that I have initially was that Mustache is a templating engine. However, after some googling, I’ve come to learn that Mustache is NOT a templating engine. Mustache is a specification for a templating language. In general, we would write templates according to the Mustache specification, and it can then be compiled by a templating engine to be rendered to create an output.

# Mustache-Express

If you intend you use mustache with Node and Express, you can use mustache-express. Mustache Express lets you use Mustache and Express together easily.

The do it step be step:
1. To Install With Yarn :
$ yarn add mustache-express
2. or With NPM :
$ npm install mustache --save
3. Configure mustache-express in your  | server.js / app.js / index.js | file:
![1_ES10lxr7tdRFVEKcRAgLEw]()
4. Create a views folder and add some html view templates (e.g. hello.html):
![1_zwYE8a5rvAVZcBl9v1oqfA]()
![1_FRcL9NQHI7Cvi2ELLmzJGQ]()
5. Then in the router configuration, use res.render(TEMPLATE_NAME, JSON_DATA). Example:
res.render('hello', {"name": "Sherlynn"})
res.render('hello', nameObject)
6. Final output :
![1_YaJ1vtsuwRMhfi8parlHOA]()

This is just a simple basic example, but I hope it helps you to understand the basic concept behind templating.

# flexbox properties

1. display

This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.

.container {
  display: flex; /* or inline-flex */
}

2. flex-direction

This establishes the main-axis, thus defining the direction flex items are placed in the flex container. Flexbox is (aside from optional wrapping) a single-direction layout concept. Think of flex items as primarily laying out either in horizontal rows or vertical columns.

.container {
  flex-direction: row | row-reverse | column | column-reverse;
}

3. flex-flow

This is a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap.

.container {
  flex-flow: column wrap;
}

4. justify-content

This defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It also exerts some control over the alignment of items when they overflow the line.

.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
}

5. align-items

This defines the default behavior for how flex items are laid out along the cross axis on the current line. Think of it as the justify-content version for the cross-axis (perpendicular to the main-axis).

.container {
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;
}

6. align-content

This aligns a flex container’s lines within when there is extra space in the cross-axis, similar to how justify-content aligns individual items within the main-axis.

.container {
  align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;
}

7. properties for the childern (flex items)

|flex items|css style|
|----------|---------|
|order|.item {
  order: 5; /* default is 0 */
}|
|flex-grow|.item {
  order: 5; /* default is 0 */
}|
|flex-shrink|.item {
  flex-shrink: 3; /* default 1 */
}|
|flex-basis|.item {
  flex-basis:  | auto; /* default auto */
}|
|flex|.item {
  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
}|
|align-self|.item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}|