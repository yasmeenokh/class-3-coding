# Review, Research, and Discussion

1. Can a parent component access the state of a child component?

In React we can access the child’s state using Refs. we will assign a Refs for the child component in the parent component. then using Refs we can access the child’s state.

2. What can be passed along in a prop variable?
props enable you to pass variables from one to another component down the component tree.

3. How can a child component “know” the state of another component?
you can pass it as a prop. Then, inside a Component you can access the data.


# Vocabulary Terms

**component props:** Keyword in React for properties, can be any information, function, JavaScript that needs to be passed to another component. Can only be passed in one direction, from the root to its children, no way for data to be passed up.

**component state:**  The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.

**application state:** In an application, state is interface between data (from backend or local change) and the representation of this data with UI elements on the front-end. State is able to keep the data of different components in sync because each state update will rerender all relevant components. State can be a medium to communicate between different components as well.

# Preparation Materials

### The Component Lifecycle :

![lifecycle](https://miro.medium.com/max/1089/1*nleLui-x8YNJhZaEwwLioQ.png)

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


### Composition vs Inheritance

* React has a powerful composition model, and we recommend using composition instead of inheritance to reuse code between components.

* In React using Composition and Props gives you all the flexibility that you would need. React does not say Composition is better than Inheritance. Composition just fits better within the React’s component structure.

* With the addition of the latest Hooks in React, re-using code is only going to be much easier.