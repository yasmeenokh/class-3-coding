# Review, Research, and Discussion

**Why is access control important?**

limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorization, unlawfully and the risk of a data breach.

**Describe an application that would need access control.**

Any E-commerce app, the admin can have the ability to change or update the prices of the products or the quantities or any information related to the products, while users have the ability to view and add the product to their basket.

**What is a role used for?**

roles are used to assigning system access to users based on their role within an organization. 

**Why is role based access control more scalable than discretionary or mandatory access control?**

RBAC better serves a company-wide security system with an overseeing administrator, by limiting unnecessary access to sensitive information based on each user’s established role within the organization.

# Vocabulary Terms

**Authorization:** is the process of giving someone permission to do or have something. ... Thus, authorization is sometimes seen as both the preliminary setting up of permissions by a system administrator and the actual checking of the permission values that have been set up when a user is getting access.

**Role Based Access Control:** RBAC, is assigning system access to users based on their role within an organization.

**Capabilities:** is a concept in the design of secure computing systems, one of the existing security models. A capability is a communicable, unforgeable token of authority. It refers to a value that references an object along with an associated set of access rights. 

# Preview 

## Event-Driven Programming in Node.js

is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

### Event-Driven Programming main concepts:

* An Event Handler is a callback function that will be called when an event is triggered.
* A Main Loop listens for event triggers and calls the associated event handler for that event.

### EventEmitter

allows us to get started incorporating Event-Driven Programming in our project right away.
All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by the object. 

We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.

    const EventEmitter = require('events').EventEmitter;
    const myEventEmitter = new EventEmitter;

### Object Oriented Programming + Event-Driven Programming

The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.

### Asynchronous vs. synchronous

The EventEmitter calls all listeners synchronously in the order in which they were registered. This ensures the proper sequencing of events and helps avoid race conditions and logic errors. When appropriate, listener functions can switch to an asynchronous mode of operation using the setImmediate() or process.nextTick() methods. 



