# Debugging

## Error Handling & Debugging

### Definition and Usage

* The debugger statement stops the execution of JavaScript, and calls (if available) the debugging function.

* Using the debugger statement has the same function as setting a breakpoint in the code.

* Normally, you activate debugging in your browser with the F12 key, and select "Console" in the debugger menu.

* The console helps narrow down the area in which the
error is located, so you can try to find the exact error.

### Note: If no debugging is available, the debugger statement has no effect.

### ERROR OBJECTS CONTINUED

[Errors](images/errors.jpg)

[Errors1](images/error1.jpg)

* HOW TO DEAL WITH ERRORS?

1. DEBUG THE SCRIPT TO FIX ERRORS
2. HANDLE ERRORS GRACEFULLY

* JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.

* If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.

## Syntax

#### debugger;










