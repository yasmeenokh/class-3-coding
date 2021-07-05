# Review, Research, and Discussion

1. How granular should your reducers be?

It is difficult to manage states that are deeply nested, so more reducers is better than only a few. Redux gives us combineReducers to let us define more precisely what our initial state will look like.

2. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

Dispatching an action within a reducer is an anti-pattern. Your reducer should be without side effects, simply digesting the action payload and returning a new state object. Adding listeners and dispatching actions within the reducer can lead to chained actions and other side effects.

3. Name a strategy for preventing the above

redux thunk

# Vocabulary Terms

**store**: is an immutable object tree in Redux. A store is a state container that holds the application’s state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer.

**combined reducers**: Helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

# Preparation Materials

### async action

Async Logic and Data Fetching React-Redux library let our React components interact with a Redux store, including calling useSelector to read Redux state, calling useDispatch to give us access to the dispatch function, and wrapping our app in a `Provider` component to give those hooks access to the store.

* a Redux store doesn’t know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.
side effects are things like:

1. Logging a value to the console.
2. Saving a file.
3. Setting an async timer.
4. Making an AJAX HTTP request.
3. Modifying some state that exists outside of a function, or mutating arguments to a function.

* Redux middleware were designed to enable writing logic that has side effects.

    * **Side effects** are code that changes state/behavior outside a function, like AJAX calls, modifying function arguments, or generating random values. 

* Middleware add an extra step to the standard Redux data flow.

    * Middleware can intercept other values passed to dispatch.

    * Middleware have access to dispatch and getState, so they can dispatch more actions as part of async logic
* The Redux “Thunk” middleware lets us pass functions to dispatch.

    * **Thunk** functions let us write async logic ahead of time, without knowing what Redux store is being used.

    * A Redux thunk function receives dispatch and getState as arguments, and can dispatch actions like “this data was received from an API response”.

