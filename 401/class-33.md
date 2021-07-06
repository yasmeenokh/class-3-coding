# Review, Research, and Discussion

1. What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?
We can wrap the opening pre-load in `useEffect`, hook to dispatch an async action which load data on application start.

2. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
We export the actual action from the reducer.



# Vocabulary Terms

**middleware**: is software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications.

**thunk**: Mainly used to delay its execution. is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.

# Preview

The **Redux Toolkit** package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

1. "Configuring a Redux store is too complicated".
2. "I have to add a lot of packages to get Redux to do anything useful".
3. "Redux requires too much boilerplate code".

* Redux Toolkit also includes a powerful data fetching and caching capability that we’ve dubbed “RTK Query”. It’s included in the package as a separate set of entry points. It’s optional, but can eliminate the need to hand-write data fetching logic yourself.

* These tools should be beneficial to all Redux users. Whether you’re a brand new Redux user setting up your first project, or an experienced user who wants to simplify an existing application, Redux Toolkit can help you make your Redux code better.

#### Redux Toolkit includes these APIs:

* `configureStore()`: wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.

* `createReducer()`: that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements. In addition, it automatically uses the immer library to let you write simpler immutable updates with normal mutative code, like state.todos[3].completed = true.

* `createAction()`: generates an action creator function for the given action type string. The function itself has toString() defined, so that it can be used in place of the type constant.

* `createSlice()`: accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.

* `createAsyncThunk()`: accepts an action type string and a function that returns a promise, and generates a thunk that dispatches pending/fulfilled/rejected action types based on that promise.

* `createEntityAdapter`: generates a set of reusable reducers and selectors to manage normalized data in the store
The createSelector utility from the Reselect library, re-exported for ease of use.

#### MobX
MobX is a simple, scalable and battle tested state management solution. This tutorial will teach you all the important concepts of MobX in ten minutes. MobX is a standalone library, but most people are using it with React and this tutorial focuses on that combination.

