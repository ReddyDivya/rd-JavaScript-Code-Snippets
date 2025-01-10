// Nested array with mixed elements
const arr = [[1, 2, [4], [3, 4]]];

// Using flat() to flatten the array by 1 level
console.log(arr.flat()); 
// Output: [1, 2, [4], [3, 4]] 
// Explanation: The array is flattened one level, but inner arrays [4] and [3, 4] remain nested.

// Nested array with deeper elements
const arr2 = [[2, 4, [2, 4], [3, 4, 2]]];

// Using flat(2) to flatten the array by 2 levels
console.log(arr2.flat(2));
// Output: [2, 4, 2, 4, 3, 4, 2]
// Explanation: This flattens the array two levels, removing the inner arrays [2, 4] and [3, 4, 2].

// Another nested array with deeper elements
const arr3 = [[11, 32, [34], [33, 4]]];

// Using flat(3) to flatten the array by 3 levels
console.log(arr3.flat(3));
// Output: [11, 32, 34, 33, 4]
// Explanation: This flattens the array three levels, removing the deepest inner arrays [34] and [33, 4].
