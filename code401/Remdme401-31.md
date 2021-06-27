# Redux - Combined Reducers

It is pulling in more than one reducer from source and creating a keyed object from them.The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

## Any reducer passed to combineReducers must satisfy these rules

1. For any action that is not recognized, it must return the state given to it as the first argument.

2. It must never return undefined. It is too easy to do this by mistake via an early return statement,
so combineReducers throws if you do that instead of letting the error manifest itself somewhere else.

3. If the state given to it is undefined, it must return the initial state for this specific reducer.
According to the previous rule, the initial state must not be undefined either.

## Using combineReducers

The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key.

Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of the state.
