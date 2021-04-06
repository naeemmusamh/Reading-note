# Sending form data

# Client/server architecture

 the web uses a client/server architecture that can be summarized as follows. a client sends a request to a server using the HTTP protocol. The server answers the request using the same protocol.

 <img src="IMAGE/client-server.png">

 An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.

# On the client side: defining how to send the data

The form element defines how the data will be sent. All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are action and method.

1. The action attribute

The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page.

- form action="https://example.com"

When specified with no attributes, as below, the <form> data is sent to the same page that the form is present.

The names and values of the non-file form controls are sent to the server as name=value pairs joined with ampersands. The action value should be a file on the server that can handle the incoming data, including ensuring server-side validation. The server then responds, generally handling the data and loading the URL defined by the action attribute, causing a new page load.

2. The method attribute

The method attribute defines how data is sent. The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method

# The GET method

The GET method is the method used by the browser to ask the server to send back a given resource: "Hey server, I want to get this resource.

Since the GET method has been used, you'll see the URL www.foo.com/?say=Hi&to=Mom appear in the browser address bar when you submit the form.

The data is appended to the URL as a series of name/value pairs. After the URL web address has ended, we include a question mark (?) followed by the name/value pairs, each one separated by an ampersand (&). In this case we are passing two pieces of data to the server.