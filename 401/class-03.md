# Review, Research, and Discussion 

## Name 3 real world use cases where you’d want to change the request with custom middleware

1. Auth middleware: every route must be authenticated if the user is not authenticated then he is not able to call the above mentioned routes,so every GET,POST calls required authentication.In this case we build a authentication middleware.

2. Error Handing Middleware: Express JS comes with default error handling params, define error-handling middleware functions in the same way as other middleware functions, except error-handling functions have four arguments instead of three.

3. Logging Middleware


## True or false: The route handler is middleware?

    true 

## In what ways can a middleware function end the process and send data to the browser?
1.      response.send()
2.      response.render()
3.      response.json()
4.      response.end()

## At what point in the request lifecycle can you “inject” middleware?
Middlewares are capable of changing requests, response objects, and can end the response cycle as well. For simplicity, you can think of middleware as a group of functions that will execute whenever a request to the server has been made.

## What can cause express to error with “Request headers sent twice, cannot start a second response?
when we are already in the Body or Finished state, but some function tried to set a header or statusCode.

# Vocabulary Terms

TERM | DETENTION 
-----|-----------------------------------------------------------
Middleware | is software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications
Request Object | The Request object retrieves the values that the client browser passed to the server during an HTTP request.
Response Object | The Response object, which contains a server's response to an HTTP request. Every HTTP request sent returns a response from the server (the Response object) which includes quite a bit of information.
Application Middleware | is software that provides services beyond those provided by the operating system to enable the various components of a distributed system to communicate and manage data. 
Routing Middleware | is used to manage these incoming requests. It kind of routes your requests to correct handler/code.
Test Driven Development | is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases. 
Behavioral Testing | is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.

# Classes
**Classes are in fact "special functions", and just as you can define function expressions and function declarations, the class syntax has two components: class expressions and class declarations.**

### How To Declare ?
One way to define a class is using a class declaration. To declare a class, you use the class keyword with the name of the class.

### Hoisting 
An important difference between function declarations and class declarations is that function declarations are hoisted and class declarations are not.

# Routing 
**refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing.**

You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function.

### Route methods
A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.
The following code is an example of routes that are defined for the GET and the POST methods to the root of the app.

### Route paths
Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.
The characters ?, +, *, and () are subsets of their regular expression counterparts. The hyphen (-) and the dot (.) are interpreted literally by string-based paths.

### Route parameters
Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.




