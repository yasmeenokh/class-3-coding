# Review, Research, and Discussion

1. Explain what a “Singleton” is (in Computer Science terms)

is a creational design pattern that lets you ensure that a class has only one instance, while providing a global access point to this instance. This is useful when exactly one object is needed to coordinate actions across the system. And to control access to some shared resource—for example, a database or a file.

2. Explain how the Singleton pattern can be used with Node modules, specifically with classes

Node.js modules can behave like Singletons, but they are not guaranteed to be always singleton.

    let cash = 0;

    const Bank = {
        deposit(amount) {
        cash += amount;
        return cash;
    },
    withdraw(amount) {
        if (amount <= cash) {
            cash -= amount;
            return true;
        } else {
            return false;
        }
    },
    total() {
        return cash;
    }
        }

    module.exports = Bank;

3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
 * write the middleware function.
 * allow the middleware access to the request and response.
 * end the cycle
 * call the next middleware.

# Vocabulary Terms

## Router Middleware
Are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. They are used to manage these incoming requests. It kind of routes your requests to correct handler/code.

## Dynamic Module Loading
is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.

## Singleton Pattern
The Singleton Pattern limits the number of instances of a particular object to just one. This single instance is called the singleton.
Singletons are useful in situations where system-wide actions need to be coordinated from a single central place. An example is a database connection pool.

## CRUD -> REST Method Matches
- C => CREATE => POST
- R => READ => GET
- U => UPDATE => PUT 
- D => DELETE => DELETE

## Mock Testing
is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones.

# Preparation Materials
## Securing Passwords:

**Cryptographic** hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

**PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM**
1. Brute Force attack
2. Hash Collision attack

## Basic Auth:
**basic access authentication** is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon.

**NOTE**
- (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.

## Authentication:
is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

### General Guidelines: 
- Make sure your usernames/user IDs are case-insensitive.
- Do NOT allow login with sensitive accounts, Do NOT use the same authentication solution
- Passwords: minimum length of 8 characters, common maximum length is 64 characters.
- Transmit passwords only over TLS (transport layer protection) or other strong transport.
- Account lockout: prevent any more login attempts after a series of failed logins.

1. Which 3 things had you heard about previously and now have better clarity on?
    1. Mock Testing
    2. Authentication
    3. Session Management 

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    1. Cryptographic
    2. basic access authentication
    3. Mock Testing
    4. Session Management

