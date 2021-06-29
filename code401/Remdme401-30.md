# Redux

The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:
"Configuring a Redux store is too complicated" "I have to add a lot of packages to get Redux to do anything useful" "Redux requires too much boilerplate code"

## installation

npx create-react-app my-app --template redux.

The ways of adding RTK to a project:

we just linked to Redux Toolkit as an individual script tag. But, in a typical application, you need to add RTK as a package dependency in your project. This can be done with either the NPM or Yarn package managers.
-Some Changes from Redux to RTK:

-import { createStore } from "redux"; +import { configureStore } from "@reduxjs/toolkit";
const store = createStore(rootReducer);
const store = configureStore({
reducer: rootReducer, +})
RTK createSlice function allows us to consolidate that logic in one place.
