# Code Snippet - 

```
foo = 30;
console.log("FOO >> "+ foo);

var foo = 100;
console.log("FOO >> "+ foo);
```

# Code Explanation: 

- Since foo is not declared with var, let, or const, it implicitly becomes a global variable. This is generally considered bad practice because it can lead to unexpected behavior in larger codebases.
- `First console.log Statement:` - This will output FOO >> 30 to the console because the global foo is accessible at this point and holds the value 30.
- `var foo = 100;` - The var keyword declares a variable that is hoisted to the top of its function or global context. This means the declaration is processed before any code is executed.
However, the assignment (foo = 100) occurs where the statement appears in the code.
- `Second console.log Statement` - This will output FOO >> 100 to the console because by this point, the variable foo has been assigned the value 100.

### Hoisting: 
The var declaration is hoisted to the top, but the assignment is not. This means the declaration exists from the start, but the initial assignment (foo = 30) and the reassignment (foo = 100) occur in sequence.

# Output
```
30
100
```
