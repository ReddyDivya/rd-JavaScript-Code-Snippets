# Code Snippets - 16

```
console.log("Age: "+ age);
var age = 26;
console.log("Age: "+ age);
```

# Code Explanation:

- `console.log("Age: "+ age);`: This line tries to log the value of the variable age to the console. However, at this point, age is declared but not yet assigned a value. In JavaScript, variable declarations are hoisted to the top of their scope, but their assignments are not. So, during this first console.log, age is hoisted to the top of its scope, but its value is still undefined. Therefore, the output of this line will be "Age: undefined".
- `var age = 26;`: This line assigns the value 26 to the variable age. Now, age has a value.
- `console.log("Age: "+ age);`: This line logs the value of age again, which is now 26. Since age has been assigned a value earlier in the code, this console.log statement will output "Age: 26".

# Output
```
Age: undefined
Age: 26
```

This behavior occurs due to hoisting, where variable declarations are moved to the top of their containing scope during the compilation phase, while their assignments remain in place.

