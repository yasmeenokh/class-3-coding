# Review, Research, and Discussion

1. Do child components have direct access to props/state from the parent?

Child components have access to state from the parent (this.state) when in a class, and have access to props as a functional component.

2. When a component “wraps” another component, how does the child component’s output get rendered?

Wrapper components are components that surround unknown components and provide a default structure to display the child components. 

3. Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?

Yes, by using composition.


4. What trick can a parent use to share all props with it’s children
The parent can pass a function to it's children, by a class or inheritance.

# Vocabulary Terms

**props.children:** can be used on components that represent generic boxes and don’t know their children ahead of time (per React docs), it is used to display whatever you include between the opening and closing tags when invoking a component.

**composition:** a development pattern based on React’s original component model where we build components from other components using explicit defined props or the implicit children prop.

# Preparation Materials

### React Children with TypeScript

#### FC type
There is a standard React type, FC, that we can use on arrow function components. FC stands for Function Component, and it aliases a type called FunctionComponent.

#### Defining the children prop type

1. **Using JSX.Element**
2. **Using ReactChild**
3. **Using ReactNode**

### A Simple React Router v4 Tutorial

React Router v4 is a pure React rewrite of the popular React package. Previous versions of React Router used configuration disguised as pseudo-components and could be difficult to understand. With v4, everything is “just components”.

#### Installation
React Router has been broken into three packages: react-router, react-router-dom, and react-router-native.

    npm install --save react-router-dom

##### The Router
THere are <BrowserRouter> and <HashRouter> components. The <BrowserRouter> should be used when you have a server that will handle dynamic requests (knows how to respond to any possible URI), while the <HashRouter> should be used for static websites.

#### History
Each router creates a history object, which it uses to keep track of the current location 1 and re-render the website whenever that changes.

#### Rendering a <Router>
Router components only expect to receive a single child element. To work within this limitation, it is useful to create an <App> component that renders the rest of your application.

#### Routes
The <Route> component is the main building block of React Router. Anywhere that you want to only render content based on the location’s pathname, you should use a <Route> element.

#### Matching paths
React Router uses the path-to-regexp package to determine if a route element’s path prop matches the current location. 

#### Creating our routes
<Route>s can be created anywhere inside of the router, but often it makes sense to render them in the same place. You can use the <Switch> component to group <Route>s. The <Switch> will iterate over its children elements (the routes) and only render the first one that matches the current pathname.
