# Programming in JavaScript - Notes Outline

## Functions

- A JavaScript function is a block of code designed to perform a particular task
- Functions can be reused
- Functions are executed when "something" invokes it (calls it)

### Defining a Function

- Functions are defined with the **function keyword, name, and parentheses ()**, in that order
- Function names can contain letters, digits, underscores, and dollar signs (same rules as variables)
- Parameters (arguments or values) should be in parentheses, separated by commas behave as local variables
- The code to be executed, by the function, is placed inside curly brackets {}

Example:
```
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

### Invoking a Function

The code inside the function will execute when "something" invokes (calls) the function, such as:
- An event occuring (user clicks a button)
- It is invoked (called) from JavaScript code
- Automatically (self invoked)

Example
```
name()
```

### Function Return

- When JavaScript reaches a return statement, the function will stop executing
- If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement
- Functions often compute a return value. The return value is "returned" back to the "caller"

Example:
```
let x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}

x result will be 12
```

