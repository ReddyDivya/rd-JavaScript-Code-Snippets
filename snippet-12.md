# Code snippet - 12


```
const name = "Sona";
let age = 26;

console.log(name.toUpperCase());
console.log(age.toString());
```

# Code Explanation:

- In JavaScript, while primitives like strings, numbers, and booleans are not objects themselves, JavaScript allows you to call methods on primitive values by implicitly wrapping them with their respective object wrapper classes.
  This process is known as `autoboxing` or `boxing`. When you call a method on a primitive value, JavaScript temporarily converts the primitive to its corresponding object wrapper,
  allows the method to be executed, and then converts it back to a primitive.

```
let name = "Sona";
console.log(name.toUpperCase());
```

- In this code snippet, name is a primitive string. When you call toUpperCase() method on name, JavaScript automatically wraps name with a String object, calls the toUpperCase() method on it, and then converts it back to a primitive string after the method call is completed.

- This behavior allows you to work with primitives in a way that feels like they are objects, providing convenient access to methods and properties defined on their respective object wrappers. However, it's important to note that these object wrappers are temporary and do not persist beyond the method call.



