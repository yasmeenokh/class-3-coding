# **Chapter 10**
## **Error handling and debugging**
 ### **Order of execution**
 * execution context:
 1. global context: one global context in any page, it is not a function.
 2. function context: code that run within a function.
 3.eval context: (NOT SHOWN)text is executed like code in an internal function called eva l ().

* variable scope:
1. global scop: any variable declared outside a function, can be used anywhere within the code.
2. function-level scope: when a variable is declared within a function.

**NOTE**
 JS reads one line of a code at a time, when data is needed from another function, it stacks the new one on the top of the current task. 

### **EXECUTION CONTEXT & HOISTING**
**Phases** 
1. prepare 
2. execute

### **UNDERSTANDING ERRORS**
1. SynatxError
2. ReferenceError
3. URIError
4. TypeError
5. RangeError
6. Error ( undefined general error)

## **Dealing with errors**
1. debug the script to fix errors: track the error and fix it
2. handel error gracefully: using try, catch, throw, and f i na 1 ly statement.

### **Using the console**
To differentiate between the types of messages you write to the console, you can use three different methods. They use various colors and icons to distinguish them.

**Examples**
1. conso1e.info() 
2. console.warn() 
3. console.error () 
4. console.table () 
5. console.assert()

## **HANDLING EXCEPTIONS**
If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.





