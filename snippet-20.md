# Code Snippet - 20

```
var variable = 10;

(() => {
  console.log(variable);//10

  variable = 20;

  console.log(variable);//20
})();//iife - immediately invoked function expression

console.log(variable);//20
var variable = 30;

```

# Code Explanation: 

- In the Memory creation phase,  the `var variable = undefined;` is stored in the memory.
- In the Code Execution Phase, the `var variable = 10;` is stored in the memory. 
- In IIFE, first, it logs `10`  in the console and re-initialized with `variable = 20;` in the memory. Then, it logs `20` in the console.
- For final `console.log(variable);` it logs `20` because it's a `var` datatype which is a global varibale.
- At last `var variable = 30;`, the variable is re-initialized with `30`.

# Output
```
10
20
20
```
