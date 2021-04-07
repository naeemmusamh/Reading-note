# Key Concepts in Positioning Elements

# Building Blocks


CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text.

1- Block-level elements

start on a new line Examples include: h1 p ul li elements tag

2- Inline elements
flow in between surrounding text Examples include: img b i elements tag

# Containing Elements

If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.


It is common to group a number of elements together inside a div element. the div element that contains this group of elements is then referred to as the containing element.

A box may be nested inside several other block-level elements. The containing element is always the direct parent of that element.

# Controll ing the Position of Elements

CSS has the following positioning schemes that allow you to control the layout of a page: 

1- normal flow

2- relative positioning

3- absolute positioning

You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.

1- normal flow :

Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.

![block1](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE/block1.jpg)

2- relative positioning :

This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed.

![block2](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE/block2.jpg)

3- absolute positioning :

This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements.

![block3](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE/block3.jpg)

To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed.

A- Fixed Positioning :

This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element.

B- Floating Elements :

Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box.

When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top.

A Fixed Width Layout :

To create a fixed width layout, the width of the main boxes on a page will usually be specified in pixels. here you can see several div elements, each of which uses an id or class attribute to indicate its purpose on the page.

a liquid layout : 

The liquid layout uses percentages to specify the width of each box so that the design will stretch to fit the size of the screen. when trying this in your browser, remember to make the window smaller and larger.

Multiple Style Sheets (@import) :

Some web page authors split up their CSS style rules into separate style sheets. some authors take an even more modular approach to stylesheets, creating separate stylesheets to control typography, layout, forms, tables, even different styles for each sub-section of a site.

Multiple Style Sheets (link) :

On this page you can see the other technique for including multiple style sheets. Inside the head element is a separate link element for each style sheet. the contents of site.css are identical to styles.css on the left hand page.