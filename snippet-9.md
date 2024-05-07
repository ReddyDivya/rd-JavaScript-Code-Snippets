# Code Snippet - 9

```
const arr = [1, [2, 3], [4, 5, 6]];
console.log(arr.toString()); //1,2,3,4,5,6
```

# Code Explanation:

- The `toString()` method converts each element of the array to a string and concatenates them, separating each element with a comma.
- The inner arrays `[2, 3]` and `[4, 5, 6]` are also converted to strings and concatenated with the outer array elements.
