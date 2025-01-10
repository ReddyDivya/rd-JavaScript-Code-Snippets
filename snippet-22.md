// An array is defined with elements 1, 2, 3, 4, 5.
const arr = [1, 2, 3, 4, 5];

// Adding a custom method `sum` to the Array prototype.
// This makes the `sum` method available to all arrays.
Array.prototype.sum = function() {
    // Use the `reduce` method to calculate the sum of array elements.
    // `acc` is the accumulator that keeps the running total.
    // `itr` is the current element being processed.
    return this.reduce((acc, itr) => {
        return acc + itr; // Add the current element to the accumulator.
    }, 0); // The initial value of the accumulator is set to 0.
};

// Call the custom `sum` method on the array `arr`.
console.log(arr.sum()); // Logs 15 (1 + 2 + 3 + 4 + 5).
