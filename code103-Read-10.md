# Call stack
is a mechanism for an interpreter to keep track of its place in a script that calls multiple functions; what function is currently being run and what functions are called from within that function.

- So when a function is called, the interpreter adds that function to call stack list, as well as any function that is called by that function. 

- If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

**NOTE**
The  call stack function is synchronous, so is done, one at a time, from top to bottom. it uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call). 

#### What causes a stack overflow?
when there is a recursive function (a function that calls itself) without an exit point. 

# JavaScript error messages && debugging

### Types of error messages
1. Reference errors
2. Syntax errors
3. Range errors
4. Type errors

## Debugging
the most common way its to simply console.log() the variables you want to check.

### Tools to avoid runtime errors
1. quokka to evaluate your code as you type
2. eslint to make sure your style guide is consistency and it will grab you an error or two along the way and. 