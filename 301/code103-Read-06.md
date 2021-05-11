# An Introduction to Node.js

## What Is Node.js?
Node.js is an event-based, non-blocking, asynchronous 1/O runtime that uses Google’s V8 JavaScript engine and libuv library.

* lets break it down and explain that as well:

**The V8 engine** is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers. It was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.

**NOTES**

1. *** How Do I Install Node.js? ***
It recommended to Version Manager. 
2. Node has excellent support for ECMAScript 2015 (ES6) and beyond. As you’re only targeting one runtime (a specific version of the V8 engine), this means that you can write your JavaScript using the latest and most modern syntax.
3. to check which node is installed, in the terminal run the following command :
    node -v
    v12.20.1

####  Introducing npm, the JavaScript Package Manager
To check which version you have installed on your system type, npm is also the world’s largest software registry 
    npm -v
    6.14.10

#### Installing a Package Locally
    npm init -y
This will create and auto-populate a package.json file in the same folder.
    npm install lodash --save

Create a file named test.js and add the following:
    const _ = require('lodash');

    const arr = [0, 1, false, 2, '', 3];
    console.log(_.compact(arr));

Back in the terminal
    node test.js
    [ 1, 2, 3 ]

## What Is Node.js Used For?

1. installing (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.
2. They can be used for anything from bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking.

## Running JS on the server via Node.js 

* The Node.js Execution Model
is single-threaded. It’s also event-driven, which means that everything that happens in Node is in reaction to an event. Under the hood, Node uses the libuv library to implement this asynchronous (that is, non-blocking) behavior.

![node](https://www.vskills.in/lms/wp-content/uploads/2019/07/image080.jpg)

#### Downsides:
1. Because it runs single thread, so blocking I/O calls should be avoided, and errors should always be handled correctly for fear of crashing the entire process.
2. The callback-based style of coding that JavaScript imposes. 

#### What Kind of Apps Is Node.js Suited To?
Node is particularly suited to building applications that require some form of real-time interaction or collaboration.

#### What Are the Advantages of Node.js?
1. speed and scalability. 
2. You can do everything in the same language. 
3. it speaks JSON. JSON is probably the most important data exchange format on the Web. 
4. JavaScript is ubiquitous: most of us are familiar with JavaScript, or have used it at some point. This means that transitioning to Node development is potentially easier than to other server-side languages.
