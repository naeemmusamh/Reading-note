# Node, Express, and APIs

What Is Node.js?

Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.

Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

# Node Is Built on Google Chrome’s V8 JavaScript Engine

The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi.It was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.

# How Do I Install Node.js?

In this next section, we’ll install Node and write a couple of simple programs. We’ll also look at npm, a package manager that comes bundled with Node.

# Node Binaries vs Version Manager

If you fancy going the version manager route, please consult our quick tip: Install Multiple Versions of Node.js using nvm. Otherwise, grab the correct binaries for your system from the link above and install those.

“Hello, World!” the Node.js Way
You can check that Node is installed on your system by opening a terminal and typing node -v. If all has gone well, you should see something like v12.14.1 displayed. This is the current LTS version at the time of writing.

Next, create a new file hello.js and copy in the following code:

console.log("Hello, World!");

This uses Node’s built-in console module to display a message in a terminal window. To run the example, enter the following command:

node hello.js

If Node.js is configured properly, “Hello, World!” will be displayed.

# Node.js Has Excellent Support for Modern JavaScript

As can be seen on this compatibility table, Node has excellent support for ECMAScript 2015 (ES6) and beyond. As you’re only targeting one runtime (a specific version of the V8 engine), this means that you can write your JavaScript using the latest and most modern syntax.

To illustrate the point, here’s a second program that makes use of several modern JavaScript features, such as tagged template literals, object destructuring and Array.prototype.flatMap():

function upcase(strings, ...values) {
  return values.map(name => name[0].toUpperCase() + name.slice(1))
    .join(' ') + strings[2];
}

const person = {
  first: 'brendan',
  last: 'eich',
  age: 56,
  position: 'CEO of Brave Software',
};

const { first, last } = person;
const emoticon = [ ['┌', '('], ['˘', '⌣'], ['˘', ')', 'ʃ'] ];

console.log(
  upcase`${first} ${last} is the creator of JavaScript! ` + emoticon.flat().join('')


Save this code to a file called index.js and run it from your terminal using the command node index.js. You should see Brendan Eich is the creator of JavaScript! ┌(˘⌣˘)ʃ output to the terminal.

# Introducing npm, the JavaScript Package Manager

As I mentioned earlier, Node comes bundled with a package manager called npm. To check which version you have installed on your system, type npm -v.

# Installing a Package Globally

Open your terminal and type the following:

npm install -g jshint

This will install the jshint package globally on your system. We can use it to lint the index.js file from the previous example:

jshint index.js

You should now see a number of ES6-related errors. If you want to fix them up, add /* jshint esversion: 6 */ to the top of the index.js file, re-run the command and linting should pass.

#Installing a Package Locally

We can also install packages locally to a project, as opposed to globally, on our system. Create a test folder and open a terminal in that directory. Next type this:

npm init -y

This will create and auto-populate a package.json file in the same folder. Next, use npm to install the lodash package and save it as a project dependency:

npm install lodash --save

Create a file named test.js and add the following:

const _ = require('lodash');

const arr = [0, 1, false, 2, '', 3];
console.log(_.compact(arr));

Finally, run the script using node test.js. You should see [ 1, 2, 3 ] output to the terminal.

# Working with the package.json File

If you look at the contents of the test directory, you’ll notice a folder entitled node_modules. This is where npm has saved lodash and any libraries that lodash depends on. The node_modules folder shouldn’t be checked in to version control, and can, in fact, be re-created at any time by running npm install from within the project’s root.

If you open the package.json file, you’ll see lodash listed under the dependencies field. By specifying your project’s dependencies in this way, you allow any developer anywhere to clone your project and use npm to install whatever packages it needs to run.

# what Is Node.js Used For?

Now that we know what Node and npm are and how to install them, we can turn our attention to the first of their common uses: installing (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.

# Node.js Lets Us Run JavaScript on the Server

Next we come to one of the biggest use cases for Node.js — running JavaScript on the server. This isn’t a new concept, and was first attempted by Netscape way back in 1994. Node.js, however, is the first implementation to gain any real traction, and it provides some unique benefits, compared to traditional languages. Node now plays a critical role in the technology stack of many high-profile companies. Let’s have a look at what those benefits are.