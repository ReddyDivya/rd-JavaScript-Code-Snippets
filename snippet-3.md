# Code Snippet - 3

```
const nestedArray = [1, [2, 3], [4, [5, 6]]];
const flattenedArray = nestedArray.flat();
console.log(flattenedArray);
```

## Explanation
- `const nestedArray = [1, [2, 3], [4, [5, 6]]]` -> Defines a nested array with three elements: `1, [2, 3], and [4, [5, 6]]`.
- `const flattenedArray = nestedArray.flat()` -> the `flat()` method to flatten the nestedArray, `creating a new one-dimensional array where all nested arrays are concatenated into it recursively`.
- `console.log(flattenedArray);` -> Outputs the flattened array to the console.

## Flattening an array
- Flattening an array refers to the process of `converting a multi-dimensional array into a one-dimensional array`.
- This process effectively `flattens` the nested structure of the array, resulting in a simpler, single-level array.

## Output
```
[1, 2, 3, 4, 5, 6]
```
