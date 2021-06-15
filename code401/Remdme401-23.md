# Routing

React Router has been broken into three packages: react-router, react-router-dom, and react-router-native.

You should almost never have to install react-router directly. That package provides the core routing components and functions for React Router applications. The other two provide environment specific components, but they both also re-export all of react-router's exports.

We are building a website, so we will install react-router-dom.

For browser based projects, there are BrowserRouter and HashRouter components.

1. The BrowserRouter should be used when you have a server that will handle dynamic requests.

2. the HashRouter should be used for static websites.


it uses to keep track of the current location and re-render the website whenever that changes. 

Router components only expect to receive a single child element.

## What does the Route render?

Routes have three props that can be used to define what should be rendered when the route’s path matches.

1. component — A React component. When a route with a component prop matches, the route will return a new element whose type is the provided React component.

2. render — A function that returns a React element 5. It will be called when the path matches.

3. children — A function that returns a React element. if the path is match or not.

when the element rendered by the Route will be passed a number of props. These will be the match object, the current location object.

