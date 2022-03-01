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
-Async keyword
-Await keyword
-Handling Errors in  Aync
