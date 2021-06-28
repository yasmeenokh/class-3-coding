# Review, Research, and Discussion

1. Describe use cases for useMemo() and useReducer().

**useReducer()** is useful when you need to use complex state logic, when you have multiple sub values, or when the next state depends on the previous state.

**Use useMemo()** runs during rendering, and it will only recompute the memoized value when one of its dependents has changed. This is an optimized way to avoid calculations every re-render.

2. Why do custom hooks need the use prefix?

Because without it will look or will be like a regular function.

3. What do custom hooks usually do?

allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.ie they give functionality that can be used across multiple components, and they are better than functions because they can access state and component lifecycle.



4. Using any list of custom hooks, research and name one that you think will be useful in your applications
useFetch hook gets us the data and the isLoading state. 


5. Describe how a hook that fetches API data might work

An API fetching hook would take in a url and any info necessary for the request and return the results of the API call. It could use a callback to update the state with the returned results.



# Vocabulary Terms

**reducer**: A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.

# Preview

## Context
Context provides a way to pass data through the component tree without having to pass props down manually at every level. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

#### When to Use Context

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component:

**NOTE**
Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

#### API

    const MyContext = React.createContext(defaultValue);

Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

#### Context.Provider
Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers. Providers can be nested to override values deeper within the tree.

#### Class.contextType
The contextType property on a class can be assigned a Context object created by React.createContext(). Using this property lets you consume the nearest current value of that Context type using this.context. You can reference this in any of the lifecycle methods including the render function.

#### Context.Consumer
A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.



