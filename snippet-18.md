# Code Snippet - 18

```
console.log("Age: "+ age);
let age = 30;
```

# Output
```
Uncaught ReferenceError: age is not defined
```

# Code Explanation:
- `console.log("Age: "+ age);`: This line attempts to log the value of the variable age to the console. However, there's a TDZ (temporal dead zone) for the age variable declared with let, which prevents access to age before its declaration. So, attempting to access age here will result in a ReferenceError because age is not yet defined within the scope of this line due to the TDZ.
- `let age = 30;`: This line declares a new variable named age using let and assigns it the value 30. This is where age is formally declared within the current scope. However, since there was an attempt to access age before its declaration in the previous line, it results in a ReferenceError due to the TDZ.

- So, the error occurs at the first line due to the temporal dead zone (TDZ) for the age variable declared with let, which prevents access to age before its declaration. Therefore, there will be no output from this code, and it will throw a ReferenceError.

