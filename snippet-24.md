// Function to calculate the sum of two numbers
function sum(a, b) {
    return a + b;
}

// Function to calculate the product of two numbers
function product(a, b) {
    return a * b;
}

// Function `op` that accepts an operation (e.g., sum or product)
// and returns a function that takes a number `a`,
// which in turn returns another function that takes a number `b`,
// and finally applies the operation on `a` and `b`.
function op(operation) {
    return function(a) { // Outer function takes `a`
        return function(b) { // Inner function takes `b`
            return operation(a, b); // Applies the operation
        };
    };
}

// Using `op` with `sum` to add 4 and 5
console.log(op(sum)(4)(5)); // Output: 9

// Using `op` with `product` to multiply 4 and 5
console.log(op(product)(4)(5)); // Output: 20

// Creating a reusable function that multiplies any number by 100
const x100 = op(product)(100); 
console.log(x100(5)); // Output: 500 (100 * 5)

// Creating a reusable function that adds 100 to any number
const p100 = op(sum)(100);
console.log(p100(5)); // Output: 105 (100 + 5)
