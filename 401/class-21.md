# Review, Research, and Discussion

1. Does a deployed React application require a server?

No you don’t need a server , It also works well when integrated into an existing server side app.

2. Why do we prefer to test a React application at the behavior rather than the unit level?

When it comes to React components you want to check how your component is rendered and if all props you pass to the component influence the behavior of your component as expected.

3. What does npm run build do?

npm run build creates a build directory with a production build of your app.

4. Describe the actual composition / architecture of a React application

React application is split into components, it is important that you can add functionality to a component without causing rippling changes through the codebase.

# Vocabulary Terms

**BDD:** behavior driven development, a branch of Test Driven Development (TDD), which uses human-readable descriptions of software user requirements as the basis for software tests.

**Acceptance Tests:** conducted to determine if the requirements of a specification or contract are met mounting.

**Mounting:** process by which the operating system makes files and directories on a storage device available for users to access via the computer’s file system.

**build:** the process of converting source code into an “executable” bundle by the browser.

# Preparation Materials

## Components and Props
Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.

### Function and Class Components

The simplest way to define a component is to write a JavaScript function, by taking a prop as an argument and returns a react element. ES6 Classes can be also used.

**Rendering a Component**
When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object. We call this object “props”.

**Note:**
1. Always start component names with a capital letter.
2. Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. A button, a form, a dialog, a screen: in React apps, all those are commonly expressed as components.
3. Extracting components is always better to enable us to have a reusable components.
4. Props are Read-Only, All React components must act like pure functions with respect to their props.

## State and Lifecycle
In addition to taking input data (accessed via this.props), a component can maintain internal state data (accessed via this.state). When a component’s state data changes, the rendered markup will be updated by re-invoking render().

State is similar to props, but it is private and fully controlled by the component.

setState() schedules an update to a component’s state object. When state changes, the component responds by re-rendering.

#### Handling Events
Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

1. React events are named using camelCase, rather than lowercase.
2. With JSX you pass a function as the event handler, rather than a string.

#### Lifecycle of Components
Each component in React has a lifecycle which you can monitor and manipulate during its three main phases.

**The three phases are:**

1. Mounting: Mounting means putting elements into the DOM.

    constructor()
    getDerivedStateFromProps()
    render()
    componentDidMount()

2. Updating: when a component is updated, a component is updated whenever there is a change in the component's state or props.

    getDerivedStateFromProps()
    shouldComponentUpdate()
    render()
    getSnapshotBeforeUpdate()
    componentDidUpdate()

3. Unmounting: when a component is removed from the DOM, or unmounting as React likes to call it.

    componentWillUnmount()


### Components and Props
Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components. You can find a detailed component API reference here.

- Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

### React Testing Library
React Testing Library (RTL) is made of simple and complete React DOM testing utilities that encourage good testing practices, especially one:

- The more your tests resemble the way your software is used, the more confidence they can give you.

- In fact, developers tend to test what we call implementation details. Let’s take a simple example to explain it. We want to create a counter that we can both increment and decrement. Here is the implementation (with a class component) with two tests: the first one is written with Enzyme and the other one with React Testing Library.
