# Why Forms?

The best known form on the web is probably the search box that sits right in the middle of Google's homepage.

In addition to enabling users to search, forms also allow users to perform other functions online. you will see forms when registering as a member of a website, when shopping online, and when signing up for newsletters or mailing lists.

1- Form Control

There are several types of form controls that you can use to collect information from visitors to your site.

A- Adding Text:

1- Text input = used for a single line of text such as email addresses and names.

2- password input = like a single line text box but it makes the character entered.

3- Text area = for longer areas of text such as messages and comments.

B- Making choices

1- Radio buttons = for use when a user must select one of of a number of options.

2- Checkbox = when a user can select and uselect one or more options.

3- Drop down boxes = when a user must pick one of a number of options from a list.

c- Submitting forms

1- submit buttons = to submit data from your from to anther web page

2- image button = similar to submit button but they allow you to use an image

D- Uploading files

1- file upload = allows user to upload files to a website

# how forms work

A user fills in a form and then presses a button to submit the information to the server.

![forms](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE\form.jpg)

# Form Structure

1-Form Structure

Form controls live inside a form element. This element should always carry the action attribute and will usually have a method and id attribute too.

action
Every form element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.

method
Forms can be sent using one of two methods: get 

With the get method, the values from the form are added to the end of the URL specified in the action attribute.
or
post

With the post method the values are sent in what are known as HTTP headers. As a rule of thumb you should use the post.

![form](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE\form1.jpg)

2- Text Input

The input element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.

name
When users enter information into a form, the server needs to know which form control each
piece of data was entered into.
The value of this attribute identifies the form control and is sent along with the information they enter to the server.

maxlength

You can use the maxlength attribute to limit the number of characters a user may enter into the text field. Its value is the number of characters they may enter.

size

The size attribute should not be used on new forms. It was used in older forms to indicate the width of the text input.

![form](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE\form2.jpg)

3- Password Input

When the type attribute has a value of password it creates a text box that acts just like a single-line text input, except the characters are blocked out. They are hidden in this way so that if someone is looking over the user's shoulder, they cannot see sensitive data such as passwords.

name

The name attribute indicates the name of the password input, which is sent to the server with the password the user enters.

size, maxlength

It can also carry the size and maxlength attributes like the the single-line text input.

![form](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE\form3.jpg)

4- Text Area

The textarea element is used to create a multi-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag. Any text that appears between the opening textarea and closing textarea tags will appear in the text box when the page loads. If the user does not delete any text between these tags, this message will get sent to the server along with whatever the user has typed.

![form](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE\form4.jpg)

5- Radio button

Radio buttons allow users to pick just one of a number of options.

name

The name attribute is sent to the server with the value of the option the user selects. When a question provides users with options for answers in the form of radio buttons, the value of the name attribute should be the same for all of the radio buttons used to answer that question.

value

The value attribute indicates the value that is sent to the server for the selected option. The value of each of the buttons in a group should be different.

checked

The checked attribute can be used to indicate which value (if any) should be selected when the page loads. The value of this attribute is checked. Only one radio button in a group should use this attribute.

Note: Once a radio button has been selected it cannot be deselected.

![form](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE\form5.jpg)

6- Check Box

Checkboxes allow users to select (and unselect) one or more options in answer to a question.

name

The name attribute is sent to the server with the value of the option the user selects. When a question provides users with options for answers in the form of checkboxes, the value of the name attribute should be the same for all of the buttons that answer that question.

value

The value attribute indicates the value sent to the server if this checkbox is checked.

checked

The checked attribute indicates that this box should be checked when the page loads. If used, its value should be checked.

![form](https://github.com/naeemmusamh/Reading-note/blob/main/IMAGE\form6.jpg)