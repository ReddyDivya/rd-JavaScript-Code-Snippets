var b = 1; // Global variable `b` is initialized to 1.

function outer() {
    var b = 2; // Declares and initializes a local `b` variable specific to `outer` with the value 2.
    
    function inner() {
        // The `b` variable declared inside `inner` is hoisted to the top of this function scope,
        // but its value is not initialized yet. At this point, `b` is `undefined`.

        console.log('b - ', b); // Logs `undefined` because the local `b` inside `inner` is hoisted but not initialized.

        b++; // Attempts to increment `b`. Since `b` is `undefined`, this operation results in `NaN`.
        console.log('b - ', b); // Logs `NaN` because `b` is now `NaN` after the increment operation.

        var b = 3; // Declares and initializes a new local `b` variable inside `inner` with the value 3.
        console.log('b - ', b); // Logs 3, the value of the local `b` declared inside `inner`.
    }
    
    inner(); // Calls the `inner` function.
}

outer(); // Calls the `outer` function, which in turn calls `inner`.
