# Review, Research, and Discussion

1. Why do we not need more .html pages in a multi-page React app?

Using react BrowserRouter allows us to navigate from one route to another, without having different html pages. Using the react-router-dom package, we can implement multiple routes in a React application. A user browsing this app feels each route is each page. So in React, multiple routes are considered as multiple pages.

2. If we wanted a component to show up on every page, where would we put it and why?

    Inside the **< BrowserRouter />**, outside a **< Route />**

3. What does props.children contain?

it is used to display whatever you include between the opening and closing tags when invoking a component.

# Vocabulary Terms

**Composition:** is a development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop.

**Children / Child Components:** A child component is a more specific part inside a parent component. Children allow you to pass components as data to other components, just like any other prop you use. The special thing about children is that React provides support through its ReactElement API and JSX

**Hash Routing:** is using the anchor part of the URL to simulate different content. For example http://site.com/#/products/list leads to displaying a list of products. We have to mention that the #/products/list bit is never sent to the server.

**Link Routing:** Provides declarative, accessible navigation around your application, to: string, to: object, to: function. **< Link>** will render a fully accessible anchor tag with the proper href.

# Preview

## Making Sense of React Hooks

#### Why Hooks?
we often can’t break complex components down any further because the logic is stateful and can’t be extracted to a function or another component. **Hooks are our best shot at solving all of these problems. Hooks let us organize the logic inside a component into reusable isolated units.** 

**NOTES:**

1. Hooks don’t introduce unnecessary nesting into your component tree. They also don’t suffer from the drawbacks of mixins.

2. Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props.

#### What Are Hooks, Exactly?
**A Hook** is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.
Hooks let you use React features (like state) from a function — by doing a single function call. React provides a few built-in Hooks exposing the “building blocks” of React: state, lifecycle, and context.

- Since Hooks are regular JavaScript functions, you can combine built-in Hooks provided by React into your own “custom Hooks”.

- Hooks are fully encapsulated — each time you call a Hook, it gets isolated local state within the currently executing component. They’re not a way to share state — but a way to share stateful logic. We don’t want to break the top-down data flow!

- Each Hook may contain some local state and side effects. You can pass data between multiple Hooks just like you normally do between functions. They can take arguments and return values because they are JavaScript functions.

- The ability to pass data between Hooks make them a great fit for expressing animations, data subscriptions, form management, and other stateful abstractions. Unlike render props or higher-order components, Hooks don’t create a “false hierarchy” in your render tree. They’re more like a flat list of “memory cells” attached to a component. No extra layers.

#### Classes:
Hooks can cover all use cases for classes while providing more flexibility in extracting, testing, and reusing code. This is why Hooks represent our vision for the future of React.

* We keep a list of Hooks per component, and move to the next item in the list whenever a Hook is used. Thanks to the Rules of Hooks, their order is the same on every render, so we can provide the component with correct state for each call. Don’t forget that React doesn’t need to do anything special to know which component is rendering — React is what’s calling your component.

#### ✌️ Rules of Hooks

* Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.
* Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions. (There is just one other valid place to call Hooks — your own custom Hooks. We’ll learn about them in a moment.)

## Using the State Hook

**function components in React look like this:**

    const Example = (props) => {
        // You can use Hooks here!
    return <div />;
    }

* We’re now introducing the ability to use React state from these, so we prefer the name “function components”.

**Note:** Hooks don’t work inside classes. But you can use them instead of writing classes.

#### What’s a Hook?

***We start by importing the useState Hook from React.***

**When would I use a Hook?**
If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component.

#### Declaring a State Variable

* In a function component, we have no this, so we can’t assign or read this.state. Instead, we call the useState Hook directly inside our component. 

**What does calling useState do?** 
It declares a “state variable”. Our variable is called count but we could call it anything else, This is a way to “preserve” some values between the function calls — useState is a new way to use the exact same capabilities that this.state provides in a class.

* The only argument to the useState() Hook is the initial state. Unlike with classes, the state doesn’t have to be an object.

* It returns a pair of values: the current state and a function that updates it. This is why we write

    const [count, setCount] = useState().

**Reading State:** In a function, we can use the variable name directly.
**Updating State:** In a function, we already have setCount and count as variables so we don’t need this. 

## Hooks at a Glance
**useState** is a Hook (we’ll talk about what this means in a moment). We call it inside a function component to add some local state to it. React will preserve this state between re-renders. It’s similar to this.setState in a class, except it doesn’t merge the old and new state together.

**Note**
You can use the State Hook more than once in a single component.

#### ⚡️ Effect Hook

Data fetching, subscriptions, or manually changing the DOM from React components before. We call these operations **“side effects”**. The Effect Hook, useEffect, adds the ability to perform side effects from a function component.   

* When you call **useEffect**, you’re telling React to run your “effect” function after flushing changes to the DOM. Effects are declared inside the component so they have access to its props and state. 

### Hooks API Reference

#### Basic Hooks
1. useState
2. useEffect
3. useContext

#### Additional Hooks

1. useReducer
2. useCallback
3. useMemo
4. useRef
4. useImperativeHandle
5. useLayoutEffect
8. useDebugValue

