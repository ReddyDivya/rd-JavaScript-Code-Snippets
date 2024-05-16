# Code Snippet - 17

```
age = 100;
console.log("Age: "+ age);
let age = 30;
console.log("Age: "+ age);
```

# Code Explanation:

- `age = 100;`: This line assigns the value 100 to the variable age. Since there's no previous declaration of age, JavaScript implicitly creates a global variable named age and assigns it the value 100.
- `console.log("Age: "+ age);`: Here, you're trying to log the value of age. However, there's a Temporal Dead Zone for the age variable declared with let, which prevents access to age before its declaration. So, despite age being implicitly declared as a global variable, the attempt to access it here results in a ReferenceError. This line will throw a ReferenceError because age is not yet defined within the scope of this line due to the TDZ.

### Temporal Dead Zone:
- The time between the let variables was hoisted and till it initialized with some value is called the Temporal Dead Zone.

### Example
```
console.log(a);// let variable is hoisted
/*
The time between the let variable and its initialization is called the Temporal Dead Zone. We can't access the variable.
*/
let a = 10;//let variable is assigned
```

### Reference Error:
- When we try to access a variable inside the Temporal Dead Zone throws a Reference Error.

- `let age = 30;`: This line declares a new variable named age using let and assigns it the value 30. This is where age is formally declared within the current scope. However, since there's already been an implicit declaration of age as a global variable, attempting to declare it again using let in the same scope will result in a syntax error.

# Output
```
Uncaught ReferenceError: Cannot access 'age' before initialization
```

So, the error occurs at the console.log statement due to the temporal dead zone (TDZ) for the age variable declared with let, which prevents access to age before its declaration. Therefore, there will be no output from this code, and it will throw a ReferenceError.
