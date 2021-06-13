# React

![React](https://img.shields.io/badge/Developer-React-informational?style=flat&logo=React&logoColor=blue&color=blue)

React is a JavaScript library, and it use something call JSX (Javascript Syntax Extension) and this JSX it produce React element.

## Why JSX ???

React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both.

React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.


### Example of React with JSX :

------------------

function formatName(user) {

  return user.firstName + ' ' + user.lastName;

}

const user = {

  firstName: 'Harper',

  lastName: 'Perez'

};

const element = (

  h1>

    Hello, {formatName(user)}!

  /h1>

);

ReactDOM.render(

  element,

  document.getElementById('root')

);

### another Example :

-------------------

const element = {

  type: 'h1',

  props: {

    className: 'greeting',

    children: 'Hello, world!'

  }

};

These objects are called “React elements”. You can think of them as descriptions of what you want to see on the screen.

---------

div id="root">/div>

We call this a “root” DOM node because everything inside it will be managed by React DOM.