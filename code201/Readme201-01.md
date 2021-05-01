# We come across all kinds of documents every day of our lives. Newspapers, insurance forms, shop catalogues... the list goes on.

Many web pages act like electronic versions of these documents. For example, newspapers show the same stories in print as they do on websites; you can apply for insurance over the web; and stores have online catalogs and commerce facilities.

In all kinds of documents, structure is very important in helping readers to understand the messages you are trying to convey and to navigate around the document. So, in order to learn how to write web pages, it is very important to understand
how to structure documents

# So in this page you well learn about:

1. Understanding structure.

2. Tags and elements

3. The evolution of HTML

4. Comments, meta information and iframe

5. HTML 5 and how old browsers understand new elements

6. How to approach building a site

7. What is HTML, CSS, and JS.

1.understanding structure. a- How Pages Use Structure. Think about the stories you read in a newspaper: for each story, there will be a headline, some text, and possibly some images. If the article is a long piece, there may be subheadings that split
the story into separate sections or quotes from those involved. Structure helps readers understand the stories in the newspaper. The structure is very similar when a news story is viewed online (although it may also feature audio or video).
This is illustrated on the right with a copy of a newspaper alongside the corresponding article on its website. The structure is very similar when a news story is viewed online. You see it like this if in paper or mobile phone:

<img src="IMAGE/201/HTML reading.jpg">

b- Structuring Word Documents The use of headings and subheadings in any document often reflects a hierarchy of information. For example, a document might start with a large heading, followed by an introduction or the most important information. This
might be expanded upon under subheadings lower down on the page. When using a word processor to create a document, we separate out the text to give it structure. Each topic might have a new paragraph, and each section can have a heading to
describe what it covers. this photo you see how structure was added to a Word document to make it easier to understand. We use structure in the same way when writing web pages.

<img src="IMAGE/201/HTML reading1.jpg">

c- HTM L Describes the Structure of Pages In the browser window you can see a web page that features exactly the same content as the Word document. To Describe the structure of a web page, we add code to the words we want to appear on the page. You can
see the HTML code for this page below. Don't worry about what the code means yet. We start to look at it in more detail on the next page. Note that the HTML code is in blue, and the text you see on screen is in black.

<img src="IMAGE/201/HTML reading2.jpg">

The HTML is made up of characters that live inside angled brackets — these are called HTML elements. Elements are usually made up of two tags: an opening tag and a closing tag. How to uses elements to describe the structure of pages??? Lets look closer
at this photo. There are several different elements. Each element has an opening tag and a closing tag.

<img src="IMAGE/201/HTML reading 3.jpg">

Tags act like containers, they tell you something about the information that lies between their opening and closing tags.

# tags and elements

## a- Body, Head & Title

1. body You met the body element in the first example we created. Everything inside this element is shown inside the main browser window. 2- head Before the body element you will often see a head element. This contains information about the page. You
will usually find a title element inside the head element. 3- title The contents of the title element are either shown in the top of the browser, above where you usually type in the URL of the page you want to visit, or on the tab for that page.

### What is HTML?????
- [ ] stands for hyper text markup language
- [ ] allows you to create links
- [ ] allows you to move from one page to another

When the web was first taking off, one of the most common ways to learn about HTML and discover new tips and techniques was to look at the source code that made up web pages. These days there are many more books and online tutorials that teach HTML, but
you can still look at the code that a web server sends to you. To try this out for yourself, simply go to this link
[HTML and CSS Book](www.htmlandcssbook.com/code/)
## The evolution of HTML

|HTML language |syntax         |
|--------------|--------------|
|HTML5         |!doctype html>|
|HTML4         |3!doctype html public “-//w3c/dtd html 4.01 transition //en” http://www.w3.org/tr/html4//loose.dtd|
|html 1.0|!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/ xhtml1-transitional.dtd">|
|xml|?xml version="1.0" ?>|
# Comments, meta information and iframe

a- Comments in html !-- --> If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters.

b- Id attribute Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore example : p id="pull quote">

c- Class attribute Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want way to identify several elements as being different from the other elements on the page. Example
            : p class="important"

d- Block elements Some elements will always appear to start on a new line in the browser window. These are known as block level elements. Example : h1>, p>, ul>, and li>. e- Inline elements Some elements will always appear to continue on the same line
as their neighboring elements. Example : a>, b>, em>, and img>.

e- Inline elements Some elements will always appear to continue on the same line as their neighboring elements. Example : a>, b>, em>, and img>.
### Grouping Text & Elements In a Block
## div
block-elements.html HTML The div element allows you to group a set of elements together in one block-level box.
Grouping Text & Elements Inline
## span
The span element acts like an inline equivalent of the div element
## IFrames
An iframe is like a little window that has been cut into your page — and in that window you can see another page.
The term iframe is an abbreviation of inline frame
