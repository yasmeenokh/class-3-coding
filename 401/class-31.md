# Review, Research, and Discussion

1. Why choose Redux instead of the Context API for global state?

It is easer when we have more complex and larger App to build, ie if you have a lot of components simultaneously updating the global state where changes made by one component might not affect most of the other components.

2. What is the purpose of a reducer?

The reducer takes in the current state , the action (which is triggered by an event), and returns the new state.

3. What does an action contain?

An action contains a type and a payload or the data to dispatch with the action.

4. Why do we need to copy the state in a reducer?
in order to keep our function pure, so we set the the new state we need to first make a copy of the previous or original state and then create anw new object to return or to update the state.


# Vocabulary Terms

**immutable state**: In object-oriented and functional programming, an immutable object (unchangeable object) is an object whose state cannot be modified after it is created. This is in contrast to a mutable object (changeable object), which can be modified after it is created.

**time travel in redux**: Time travel is the ability to move back and forth among the previous states of an application and view the results in real time. With Redux, given a specific state and a specific action, the next state of the application is always exactly the same.

**action creator**: a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store’s dispatch() function.

**reducer**: A reducer is a function that determines changes to an application’s state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application’s state changes in a single store so that they behave consistently.

**dispatch**: dispatch() is the method used to dispatch actions and trigger state changes to the store. react-redux is simply trying to give you convenient access to it. Note, however, that dispatch is not available on props if you do pass in actions to your connect function.

# Preview

## Using combineReducers

### Core Concepts:

* The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

* Because this pattern is so common, Redux provides the combineReducers utility to implement that behavior. It is an example of a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.

*  In order to assemble the new state tree, combineReducers will call each slice reducer with its current slice of state and the current action, giving the slice reducer a chance to respond and update its slice of state if needed. So, in that sense, using combineReducers does "call all reducers", or at least all of the slice reducers it is wrapping.

* The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore. The state produced by `combineReducers()` namespaces the states of each reducer under their keys as passed to `combineReducers()`. 





