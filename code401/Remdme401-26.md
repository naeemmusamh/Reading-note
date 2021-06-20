# React Hook

## use Toggle

it takes a parameter with value true or false and toggles that value to opposite. It's useful when we want to take some action into it's opposite action, for example: show and hide modal, show more/show less text, open/close side menu.

## use Fire store Query

method you simply pass a query to it and you get back everything you need, including status, data, and error. Your component will re-render when data changes and your subscription will be automatically removed when the component unmounts.

## use Memo Compare

This hook is similar to useMemo, but instead of passing an array of dependencies we pass a custom compare function that receives the previous and new value. The compare function can then compare nested properties, call object methods, or anything else to determine equality.

## use Async

It's generally a good practice to indicate to users the status of any async request.

## use Require Auth

A common need is a way to redirect the user if they are signed out and trying to view a page that should require them to be authenticated.

## use Event Listener

is hook that handles checking if addEventListener is supported, adding the event listener, and removal on cleanup.

## use DarkMode

This hook handles all the stateful logic required to add a ☾ dark mode toggle to your website.

# React Hook you should have it in your Toolbox

* use Array hook

Adding elements to an array or removing an element at a given index.

to install it (npm i react-hanger)

to use it (import {useArray} from 'react-hanger')

* react use form state hook

managing the form state

to install it (npm i react-use-form-state)

to use it (import {useFormState} from 'react-use-form-state')

* react Fetch hook

making ajax calls is like the most basic and most performed task fpr a frontend developer.

to install it (npm i react-fetch-hook)

to use it (import {useFetch} from 'react-fetch-hook')

* use media hook

React sensor hook that tracks the sate of a CSS media query.

to install it (it will download with the use Effect)

to use it (import {useMedia} from 'use-media')
