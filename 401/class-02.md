# Review, Research, and Discussion

## What’s the Difference between PUT vs PATCH?

### PUT: 
is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely. PUT is similar to POST in that it can create resources, but it does so when there is a defined URI. PUT overwrites the entire entity if it already exists, and creates a new resource if it doesn’t exist.

### PATCH: 
applies a partial update to the resource. This means that you are only required to send the data that you want to update, and it won’t affect or change anything else.

#### Similarities
They can both be used to update resources in a given location.

#### Differences 
* The way the server processes the enclosed entity to update the resource identified by the Request-URI. When making a PUT request, the enclosed entity is viewed as the modified version of the resource saved on the original server, and the client is requesting to replace it. However, with PATCH, the enclosed entity boasts a set of instructions that describe how a resource stored on the original server should be partially modified to create a new version.

## 3 services or tools that allow you to “mock” an API for development
1. Postman 
2. MockServer
3. Wiremock

## Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

**apiDocjs:** Inline Documentation for RESTful web APIs. It creates a documentation from API annotations in your source code. It includes a default template which uses handlebars, Bootstrap, RequireJS and jQuery for the output of the generated apidata.js and apiproject.js as a html-page.

**Swagger Inspector:** Test and Document Your APIs With Ease. It is a free cloud-based API testing and documentation tool to simplify the validation of any API and generate its corresponding OpenAPI documentation.

- swagger use plain .json that could be parsed through programing language, thus we can get advantage of various other 3rd parties in order to create http client and more. 

-  apidocjs and swagger both required documentation content on implemented method as customize comment data. In addition they allow to write documentation data in separate resource file as .js and .json. If we already have swagger.json created by DotnetCore we can reuse more than 80% specification.

## Compare and contrast SOAP and ReST
1. SOAP stands for Simple Object Access Protocol whereas REST stands for Representational State Transfer.
2. SOAP is a protocol whereas REST is an architectural pattern.
3. SOAP uses service interfaces to expose its functionality to client applications while REST uses Uniform Service locators to access to the components on the hardware device.
4. SOAP needs more bandwidth for its usage whereas REST doesn’t need much bandwidth.
5. SOAP only works with XML formats whereas REST work with plain text, XML, HTML and JSON.
6. SOAP cannot make use of REST whereas REST can make use of SOAP.

## Vocabulary Terms

**Web Server**: can refer to hardware or software, or both of them working together. On the hardware side, a web server is a computer that stores web server software and a website's component files. A web server connects to the Internet and supports physical data interchange with other devices connected to the web. On the software side, a web server includes several parts that control how web users access hosted files. At a minimum, this is an HTTP server. 

**Express**: is a back end web application framework for Node.js, released as free and open-source software under the MIT License. It is designed for building web applications and APIs.[3] It has been called the de facto standard server framework for Node.js

**Routing**: is the process of selecting a path for traffic in a network or between or across multiple networks. Broadly, routing is performed in many types of networks, including circuit-switched networks, such as the public switched telephone network (PSTN), and computer networks, such as the Internet.

**WRRC**: The request/response cycle traces how a user's request flows through the app. Understanding the request/response cycle is helpful to figure out which files to edit when developing an app (and where to look when things aren't working).

## Preparation Materials

### Express/Node introduction
**NODE** : s an open-source, cross-platform runtime environment that allows developers to create all kinds of server-side tools and applications in JavaScript. The runtime is intended for use outside of a browser context.
**Node Advantages**
1. Node was designed to optimize throughput and scalability in web applications and is a good solution for many common web-development problems.
2. Code is written in plain old JavaScript.
3. JavaScript is a relatively new programming language and benefits from improvements in language design when compared to other traditional web-server languages.
4. The node package manager (NPM) provides access to hundreds of thousands of reusable packages.
5. Node.js is portable.

**Express**: the most popular Node web framework, and is the underlying library for a number of other popular Node web frameworks. 

#### Why Express?
1. Write handlers for requests with different HTTP verbs at different URL paths (routes).
2. Integrate with "view" rendering engines in order to generate responses by inserting data into templates.
3. Set common web application settings like the port to use for connecting, and the location of templates that are used for rendering the response.
4. Add additional request processing "middleware" at any point within the request handling pipeline.

### What is NPM ?
npm is the world's largest software registry. Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well.

#### components:
1. website: to discover packages, set up profiles, and manage other aspects of your npm experience
2. Command Line Interface (CLI): runs from a terminal, and is how most developers interact with npm.
3. registry: is a large public database of JavaScript software and the meta-information surrounding it.

#### When to use : 
* Adapt packages of code for your apps, or incorporate packages as they are.
* Download standalone tools you can use right away.
* Run packages without downloading using npx.
* Share code with any npm user, anywhere.
* Restrict code to specific developers.
* Create organizations to coordinate package maintenance, coding, and developers.
* Form virtual teams by using organizations.
* Manage multiple versions of code and code dependencies.
* Update applications easily when underlying code is updated.
* Discover multiple ways to solve the same puzzle.
* Find other developers who are working on similar problems and projects.

## What is TDD? 
**Definition**: “Test-driven development” refers to a style of programming in which three activities are tightly interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring).

#### set of rules:

* write a “single” unit test describing an aspect of the program
* run the test, which should fail because the program lacks that feature
* write “just enough” code, the simplest possible, to make the test pass
* “refactor” the code until it conforms to the simplicity criteria
* repeat, “accumulating” unit tests over time

## Continuous Integration Continuous Delivery

Continuous integration (CI) and continuous delivery (CD) embody a culture, set of operating principles, and collection of practices that enable application development teams to deliver code changes more frequently and reliably. The implementation is also known as the CI/CD pipeline.

