# Code Snippet 15:

```
(function() {
  var a = b = 3;
})();

console.log(typeof a);//undefined
console.log(typeof b);//number

console.log(window.a);//undefined
console.log(window.b);//3

console.log(typeof a !== "undefined");//false
console.log(typeof b !== "undefined");//true
```

# Output
```
undefined
number

undefined
3

false
true
```

# Code Explanation:

### Immediately Invoked Function Expression (IIFE):
- This code defines an immediately invoked function expression (IIFE), which is a function that is declared and immediately invoked. It's used here to create a local scope.

### Variable Declaration:
- Inside the function, there's a variable declaration: var a = b = 3;.
- Due to the right-to-left associativity in JavaScript, this statement is interpreted as b = 3 followed by var a = b;.
- Since var is used only for a, a is scoped to the function, but b is not declared with var, let, or const, making it global.

### console.log():
After the IIFE, there are several console.log() statements to log the types and values of variables a and b.

### Output Analysis:
- console.log(typeof a);: This will output "undefined" because a is scoped to the function and is not accessible outside of it.
- console.log(typeof b);: This will output "number" because b is not scoped to the function and has been assigned the value 3 globally.
- console.log(window.a): This will output undefined because a is not added to the global scope.
- console.log(window.b): This will output 3 because b has been assigned a global value of 3.
- console.log(typeof a !== "undefined"): This will output false because a is indeed undefined.
- console.log(typeof b !== "undefined"): This will output true because b is defined globally.

### Output
```
undefined
number
undefined
3
false
true
```
In summary, a is undefined outside of the function scope, while b is defined globally and holds the value 3.
