# Review, Research, and Discussion

1. Name 5 Javascript UI Frameworks (other than React)

* Angular Material
* NGX Bootstrap
* Webix
* Vue
* Base web

2. What’s the difference between a framework and a library?

When you call a method from a library, you are in control. But with a framework, the control is inverted: the framework calls you.

with **framework**; the framework is in charge of the flow. It provides you with a few places to plug in your code, but it calls the code you plugged in as needed. With a **library**; you are in charge of the application flow. You choose when and where to call the library.

# Vocabulary Terms

**Rendering:** is the act of generating a frame from your app and displaying it on the screen. the data is retrieved from the server, and processed at the browser to display to the user.



**Templates:** They are made up of common user interface elements such as buttons and navigation. They typically include core elements like icons, typography, colors, and sometimes complex UI patterns like grids, cards, and navigation. They are used to create mockups or prototypes of product solutions.

**State:**  is a data structure comprising: events. control states. an extended state variable. transitions between control states mapped to actions to be executed as a result of an event triggering the transition.


# Preview 

1. Which 3 things had you heard about previously and now have better clarity on?
framework and Templates. 

2. What are you most excited about trying to implement or see how it works?
React. 

# Preparation Materials

## Introducing JSX
it is a syntax extension to JavaScript. It describe what the UI should look like. 

##### Why JSX?
Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both.

**Embedding Expressions in JSX** 
Example:

    const name = 'Josh Perez';
    const element = <h1>Hello, {name}</h1>;

    ReactDOM.render(
        element,
        document.getElementById('root')
    );

**Notes:**
1. You can use JSX inside of if statements and for loops, assign it to variables, accept it as arguments, and return it from functions.
2. You can use quotes to specify string literals as attributes.
3. You can use curly braces to embed a JavaScript expression in an attribute.
4. **JSX Prevents Injection Attacks**.
5. **JSX Represents Objects.**

## Rendering Elements
An element describes what you want to see on the screen. React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

- To render a React element into a root DOM node, pass both to ReactDOM.render().

##### Updating the Rendered Element
React elements are immutable. Once you create an element, you can’t change its children or attributes. 

With our knowledge so far, the only way to update the UI is to create a new element, and pass it to ReactDOM.render().

**React Only Updates What’s Necessary**.





