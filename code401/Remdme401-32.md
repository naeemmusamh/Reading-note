# Redux Thunk middleware

Redux Thunk middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. The inner function receives the store methods dispatch and getState as parameters.

Thunks are the recommended middleware for basic Redux side effects logic, including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests.

## Basic Usage

The most common use-case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.

## What is React Suspense?

Suspense is a new React feature that was announced recently at the JSConf Conference in Iceland. It aims to help with handling async operations respectively in regard to CPU power and data fetching.
