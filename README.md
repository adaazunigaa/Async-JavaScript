# Async JavaScript
-The Call Stack
    *Mechanism the JS interpreter uses to keep track of its place in a scrip that calls multiple functions.
    It is how JS "knows" what function is currently being run and what functions are called from within that function
           HOW IT WORKS 
    -When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function
    -Any functions that are called by that function are added to the call stack further up, and rrun where their calls are reached
    -When the current funcntion is finished, the interpreter tales it off the stacj and reumes execution where  it left off in the last code listing
-Web API's and Single Threaded
    SINGLE THREADED
        *At any given point in time, that single JS thread is tunning at most one line of JS code
    API's ??
        *Browser comes with API's that are able to handle certain task in the background (like making requests or setTimeout)
        *The JS call stack recognizes these Web API's functions and passes them off to the browser to take care of
        *Once the browser finishes those task, they return and are pushed onto the stack as a callback
-Callback
-Promises
    A "Proimise" is an object representing the eventual completion of failure of an asynchronous operation 
    -Apromise is a returned object to which you attach callbacks, instead of passing callbacks into a dunction
-Async keyword
    *-Async functions always return a promise 
     -If the function returns a calue, the promise will be resolved with that value
     -If the function throws an exception, the promise will be rejected 

    *ASYNC FUNCTIONS:
        Newer and cleaner syntax for working with async code 
        Syntax "makeup" for promises
    
-Await keyword
    *Mostly inside of functions declared with async 
    *Await will pause the execution of the function, waiting for a promise to be resolved.
-Handling Errors in  Aync
