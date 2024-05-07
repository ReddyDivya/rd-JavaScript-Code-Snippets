# Code Snippet - 10

```
console.log([2, 3, [6,7]].toString());//2,3,6,7
console.log(2, 3, [6,7].toString());//2 3 6,7
console.log(2 .toString());//2
console.log((2).toString());//2
console.log(2..toString());//2
```

# Code Explanation:

`console.log([2, 3, [6,7]].toString());`: 
- This line creates an array [2, 3, [6,7]].
- The toString() method is called on this array, converting each element to a string and concatenating them with commas separating each element.
- `Output: "2,3,6,7"`

`console.log(2, 3, [6,7].toString());`:
- This line logs three values to the console: 2, 3, and [6,7].toString().
- The number 2 and 3 are logged directly.
- [6,7].toString() is called, resulting in "6,7", which is then logged.
- Output: "2 3 6,7"

`console.log(2 .toString());`:
- This line logs the result of calling toString() on the number 2.
- There's a space between 2 and the dot, which ensures that JavaScript doesn't interpret 2. as a floating-point number.
- Output: "2"
  
`console.log((2).toString());`:
- This line logs the result of calling toString() on the number 2.
- The parentheses around 2 ensure that JavaScript treats 2 as a number literal and then applies the toString() method to it.
- Output: "2"

`console.log(2..toString());`:
- This line logs the result of calling toString() on the number 2.
- The two dots (2..) ensure that JavaScript doesn't interpret 2. as a floating-point number.
- Output: "2"

These examples illustrate different ways of calling the toString() method on numbers and arrays, along with handling syntax to avoid potential issues with parsing numbers in JavaScript.
