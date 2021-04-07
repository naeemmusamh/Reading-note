# JQUERY

WHAT IS JQUERY

Jquery is a JavaScript file that you include in your web pages. it lets you file element using CSS-Style selectors and then do something with the elements using jquery methods.

a function called jquery() lets you find one or more elements in the page.
it creates an object called jquery which holds references to those elements.
$() is often used as a shourthand to save types jquery().

![jquery](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE/jquery.jpg?raw=true)

the jquery object has many methods that you can use to work with the elements you select. the methods represent tasks that you commonly need to perform with eleements.
 
 ![jquery](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE/jquery1.jpg?raw=true)

A BASIC JQUERY EXAMPLE

The examples in this chapter revisit the list application used in the previous two chapters, and they will use jQuery to update the content of the page.

1. In order to use jQuery, the first thing you need to do is include the jQuery script in your page. You can see that it is included before the closing body tag element.

2. Once jQuery has been added to the page, a second JavaScript file is included that uses jQuery selectors and methods to update the content of the HTML page.

WHERE TO GET JQUERY AND WHICH VERSION TO USE

jQuery is included before the closing </ body> tag just like other scripts.

If you want to look at the jQuery file, you can open it with a text editor - it is just text like JavaScript, albeitver complicated JavaScript.

Most people who use jQuery do not try to understand how the jQuery JavaScript file achieves what it does.As long as you know how to select elements and how to use its methods and properties, you can reap the benefits of using jQuery without looking under the hood.

![jquery](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE/jquery2.jpg?raw=true)

![jquery](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE/jquery11.jpg?raw=true)

WHY USE JQUERY?

jQuery doesn't do anything you cannot achieve with pure JavaScript. It is just a JavaScript file but estimates show it has been used on over a quarter of the sites on the web, because it makes coding simpler.

jQuery's motto is "Write less, do more," because it allows you to achieve the same goals but in fewer lines of code than you would need to write with plain JavaScript.

# A MATCHED SET / JQUERY SELECTION

when you select one or more elements, a jquery object is returned. it is also known as a matched set or a jquery selection.

1. single element
if a selector returns one ele,ent, the jquery object contains a reference to just one element node.

2. multiple element
if a selector returns several elements the jquery object contains references to each element.

some jquery methods both retieve information from and update the contents of element. but they do not always apply to all elements.

1. get information
if a jquery holds more than one element and a method is used to get information from the select element it wil retrieve information from only the first element in the matched set

2. set information
if a jquery holds more than one element and a method is used to update information on the page it will update all of the element in the matched set not just the first one.

![jquery](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE/jquery3.jpg?raw=true)

