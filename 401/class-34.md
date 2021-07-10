# Review, Research, and Discussion

1. Compare and Contrast Redux Toolkit with Redux “Ducks”
Ducks is a way to bundle reducers, action types, and actions into the same file. Rather than splitting up related code, it can be packaged into redux modules.

Redux Toolkit goal is to help simplify common Redux use cases. It is not intended to be a complete solution for everything you might want to do with Redux, but it should make a lot of Redux-related code you need to write a lot simpler. Redux Toolkit exports several individual functions that you can use in your application, and adds in dependencies on some other packages that are commonly used with Redux.

2. What is the principle advantage of Redux Toolkit?
Helps to solve three major problems with Redux: configuring a Redux store, adding numerous packages to get Redux to things, and removing unnecessary or boilerplate code.

# Vocabulary Terms

**redux toolkit slices**: A function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state.

**namespace**: Programming paradigm of providing scope to identifiers (names of types, functions, variables, etc) to prevent collisions between them. JavaScript does not provide namespace by default. However, we can replicate this functionality by making a global object which can contain all functions and variables.


# Preparation Material 

## React Native 

React Native is an open source framework for building Android and iOS applications using React and the app platform’s native capabilities. With React Native, you use JavaScript to access your platform’s APIs as well as to describe the appearance and behavior of your UI using React components: bundles of reusable, nestable code.

### Views and mobile development

**view**: is the basic building block of UI: a small rectangular element on the screen which can be used to display text, images, or respond to user input. Even the smallest visual elements of an app, like a line of text or a button, are kinds of views. Some kinds of views can contain other views.

**NOTES**

* React Native lets you create truly native apps and doesn't compromise your users' experiences. It provides a core set of platform agnostic native components like View, Text, and Image that map directly to the platform’s native UI building blocks.

* React components wrap existing native code and interact with native APIs via React’s declarative UI paradigm and JavaScript. This enables native app development for whole new teams of developers, and can let existing native teams work much faster.

### React Native Advantages: 
Optimal Performance, Code Reusability, Large Community, Cost Effective, Modular Architecture, Hot Reloading Support, Simple User Interface, Offers More Stable Apps, Third-Party Plugins Support, and Handy Solutions & Libraries.

## Introduction to Expo

Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.