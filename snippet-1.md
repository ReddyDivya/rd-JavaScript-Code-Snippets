# Code Snippet 1:

## Converts number to a string
```
const data = 100;
console.log(data.toString());//converts number to a string
```

## Directly converts number to a string

```
console.log(100.toString());//Uncaught SyntaxError: Invalid or unexpected token
```

## To fix the syntax error:
- `console.log(100.toString());` : Tries to directly convert the number 100 to a string using the toString() method. 
- However, this will result in a syntax error because JavaScript interprets the dot following 100 as a decimal point, not as a property accessor.
- To fix this, we would need to use parentheses to ensure proper parsing: `console.log((100).toString());`.
- Another way, when we have a number followed by two dots like `100..toString()`, it's a way to explicitly specify that we're dealing with a number, not a decimal point.
- So, `console.log(100..toString())`; is valid JavaScript syntax and it correctly converts the number 100 to a string using the toString() method.

---

