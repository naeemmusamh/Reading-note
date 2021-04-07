# image

1. Controlling sizes of images in CSS

You can control the size of an image using the width and height properties in CSS, just like you can for any other box.

Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download.

<img src="IMAGE\image1.jpg">

2. Aligning images using CSS

using the img element's align attribute, web page authors are increasingly using the float property to align images.

There are two ways that this is commonly achieved:
1. The float property is added to the class that was created to represent the size of the image.
2. New classes are created with names such as align-left or align-right to align the images to the left or right of the page.

<img src="IMAGE\image2.jpg">

3. Centering images using CSS

images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a block level element using the display property with a value of block.

<img src="IMAGE\image3.jpg">

4. Background-images

The background-image property allows you to place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image will repeat to fill the entire box. The path to the image follows the letters url, and it is put inside parentheses and quotes.

<img src="IMAGE\image4.jpg">

5. Repeating images

The background-repeat property can have four values:
1- repeat :
The background image is repeated both horizontally and vertically.
2- repeat-x :
The image is repeated horizontally only.
3- repeat-y :
The image is repeated vertically only.
4- no-repeat :
The image is only shown once.

The background-attachment property specifies whether a background image should stay in one position or move as the user scrolls up and down the page. It can have one of two values:
1- fixed :
The background image stays in the same position on the page.
2- scroll :
The background image moves up and down as the user scrolls up and down the page.

<img src="IMAGE\image5.jpg">

6. background position 

When an image is not being repeated, you can use the background-position property to specify where in the browser window the background image should be placed.
This property usually has a pair of values. The first represents the horizontal position and the second represents the vertical.

(left top ,left center ,left bottom ,center top ,center center ,center bottom ,right top ,right center ,right bottom)

<img src="IMAGE\image6.jpg">
<img src="IMAGE\image7.jpg">

7. shorthand

The background property acts like a shorthand for all of the other background properties you have just seen, and also the background-color property.
The properties must be specified in the following order, but you can miss any value if you do not want to specify it.

1: background-color
2: background-image
3: background-repeat
4: background-attachment
5: background-position

8. image rollovers & sprites

Using CSS, it is possible to create a link or button that changes to a second style when a user moves their mouse over it and a third style when they click on it.

# PRACTICAL INFORMATION

# Search Engine Optimization (SEO)

SEO is a huge topic and several books have been written on the subject. The following pages will help you understand the key concepts so you can improve your website's visibility on search engines.

1. The Basics
is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics that your website covers.
2. On-Page Techniques
On-page techniques are the methods you can use on your web pages to improve their rating in search engines.
3. Off-Page Techniques
Getting other sites to link to you is just as important as on-page techniques. Search engines help determine how to rank your site by looking at the number of other sites that link to yours.

In every page of your website there are seven key places where keywords can appear in order to improve its findability.

1. Page Title :
The page title appears at the top of the browser window or on the tab of a browser. It is specified in the title element which lives inside the head element.

2. URL / Web Address :
The name of the file is part of the URL. Where possible, use keywords in the file name.

3. Headings :
If the keywords are in a heading hn element then a search engine will know that this page is all about that subject and give it greater weight than other text.

4. Text :
Where possible, it helps to repeat the keywords in the main body of the text at least 2-3 times. Do not, however, over-use these terms, because the text must be easy for a human to read.

5. Link Text :
Use keywords in the text that create links between pages.

6. Image Alt Text :
Search engines rely on you providing accurate descriptions of images in the alt text. This will also help your images show up in the results of image-based searches.

7. Page Descriptions :
The description also lives inside the head element and is specified using a meta tag. It should be a sentence that describes the content of the page.

# How to Identify Keywords and Phrases

Determining which keywords to use on your site can be one of the hardest tasks when you start to think about SEO. Here are six steps that will help you identify the right keywords and phrases for your site.

1. Brainstorm
List down the words that someone might type into Google to find your site. Be sure to include the various topics, products or services your site is about.

2. Organize
Group the keywords into separate lists for the different sections or categories of your website.

3. Research
There are several tools that let you enter your keywords and then they will suggest additional keywords you might like to consider.

4. Compare
It is very unlikely that your site will appear at the top of the search results for every keyword. This is especially true for topics where there is a lot of competition.

5. Refine
Now you need to pick which keywords you will focus on. These should always be the ones that are most relevant to each section of your site.

6. Map
Now that you have a refined list of keywords, you know which have the most competition, and which ones are most relevant, it is time to start picking which keywords you will use for each page.