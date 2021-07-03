# Review, Research, and Discussion

1. What are the advantages of storing tokens in “Cookies” vs “Local Storage”?

The cookie is not accessible via JavaScript; hence, it is not as vulnerable to XSS attacks as localStorage.

2. Explain 3rd party cookies.

are cookies that are set by a website other than the one you are currently on. 

3. How do pixel tags work?

is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage or opens an email. The website operator or sender of an email adds the tracking pixel using a code in the website’s HTML code or email. This code contains an external link to the pixel server. If a user visits the destination website, the HTML code is processed by the client – usually the user’s browser. The browser follows the link and opens the (invisible) graphic. This is registered and noted in the server’s log files.

# Vocabulary Terms

**cookies**: are small blocks of data created by a web server while a user is browsing a website and placed on the user's computer or other device by the user’s web browser. Cookies are placed on the device used to access a website, and more than one cookie may be placed on a user’s device during a session.

**authorization**:  is the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular. 

**access control**: he control of access to system resources after a user’s account credentials and identity have been authenticated and access to the system has been granted.

**conditional rendering**: you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.

# Preview: 

## Redux

**What is a redux**
Redux provides a solid, stable, and mature solution to managing state in your React application. Through a handful of small, useful patterns, Redux can transform your application from a total mess of confusing and scattered state, into a delightfully organized, easy to understand modern JavaScript powerhouse.

**A Predictable State Container for JS Apps**

**Why use Redux?**
Some of the nice things you get with using Redux include logging, hot reloading, time travel, universal apps, record and replay — all without doing so much on your end as the developer. These things will likely sound fancy until you use them and see for yourself.
The Redux Store can be likened to the Bank Vault. It holds the state of your application — and keeps it safe.

**Benefits of redux:**
* When we have large amounts of application state that are needed in many places in the app.

* When the app state is updated frequently over time.

* When the logic to update that state may be complex.

* When the app has a medium or large-sized codebase, and might be worked on by many people

### Redux Principles:

**First Principle:** The state of the application will be saved in a single Js object.

**Second Principle:** The state tree is redundant, ie you can't modify it or update it, the only way to change the tree is by transmitting an action.

**Note**
An action is a plain js object describing what changed in the app, wether it was initiated by a network request or user interaction. any data that enters the redux app gets their by actions.

**Third Principle:** The state mutations in the app needs to be described in **pure functions**, that takes the previous state and the actions being dispatched and then returns the next state. This function is called the **Reducer**.

### CreateStore:
it combines the three principles of redux, it holds the current state, and you need to specify the reducer. It has three main methods:

1. getState(): retrieves the current state.

2. **dispatch()**: which will let dispatch actions to change the action. Which takes the action type as an argument.

3. subscribe(): it lets you call, a callBack function anytime an action has been dispatched to change the UI
