# Learn Javascript from Scratch

## Difference between these two code snippet        
```javascript
    function greetStudent(name){
    console.log(`Welcome, ${name}`);
}
let greet= greetStudent("AJay");
greet;
```
> The greet here shows undefined because of implicit return of function

and 
```javascript
    function greetStudent(name){
        return(`Welcome, ${name}`);
    }
    let greet= greetStudent("AJay");
    greet;
```

The main difference between the two code snippets is the use of the `console.log` statement in the first snippet and the `return` statement in the second snippet.

In the first snippet:
```javascript
function greetStudent(name){
    console.log(`Welcome, ${name}`);
}
let greet = greetStudent("AJay");
```
The `greetStudent` function is defined with a parameter `name`, and it uses `console.log` to print a welcome message to the console, including the provided name. When the function is called with the argument "AJay", it immediately logs the message "Welcome, AJay" to the console. The variable `greet` is assigned the value `undefined` because the function does not explicitly return any value.

In the second snippet:
```javascript
function greetStudent(name){
    return(`Welcome, ${name}`);
}
let greet = greetStudent("AJay");
greet;
```
The `greetStudent` function is defined in the same way as before, but instead of using `console.log`, it uses the `return` statement to return a string containing the welcome message. When the function is called with the argument "AJay", it evaluates the `return` statement and produces the string "Welcome, AJay" as the result. The variable `greet` is assigned this returned value. Finally, the value of `greet` is evaluated and output to the console, which will display "Welcome, AJay".

In summary, the difference is that the first snippet immediately logs the welcome message to the console, while the second snippet returns the welcome message as a value that can be assigned to a variable or used in other parts of the code.
