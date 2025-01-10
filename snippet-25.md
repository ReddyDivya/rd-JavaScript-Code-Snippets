const deeplyNested = [1, [2, [3, [4, [5]]]]];

// Without flat()
console.log(deeplyNested); 
// Output: [1, [2, [3, [4, [5]]]]]

// Using flat(Infinity)
console.log(deeplyNested.flat(Infinity)); 
// Output: [1, 2, 3, 4, 5]
