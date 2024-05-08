# Code Snippet - 6

# Simple Thread on JavaScript setTimeout in a Loop🧵

```
for(var i=0; i<10; i++)
{
  setTimeout(() => {
    console.log(i)
  }, 8);
}
```

# Code Explanation:

In this code snippet, it seems like you're attempting to print numbers from 0 to 9 with a delay of 100 milliseconds between each number. However, due to the asynchronous nature of JavaScript and the behavior of closures, the output is unexpected.

Let's break down what's happening:

`for loop`:
- The for loop runs 10 iterations, with i starting at 0 and incrementing by 1 until it reaches 9 (i < 10).

`setTimeout function`:
- Inside the loop body, a setTimeout function is called. This function schedules a task to be executed after a specified delay (100 milliseconds in this case). The task is defined by the arrow function provided as the first argument to setTimeout.
However, due to the asynchronous nature of setTimeout, it does not block the execution of the loop. Instead, it schedules its callback function to be executed after the specified delay, and the loop continues to run immediately.

`Closure and Variable Scope`:
- The setTimeout callback function captures the reference to the variable i from its surrounding environment. Since JavaScript has function-level scope (prior to ES6) and the loop variable i is declared with var, there is only one variable i shared across all iterations of the loop.
- By the time the setTimeout callbacks are executed (after the delay), the loop has already completed, and the final value of i is 10.

### Output:
- When the setTimeout callbacks are executed, they access the value of i from the outer scope. Since the loop has completed, the value of i is 10 at this point for all the callbacks.
Therefore, each callback prints the value of i, which is 10, resulting in "10" being printed 10 times.

10
10
10
10
10
10
10
10
10
10

- To fix this issue and print numbers from 0 to 9 with a delay of 100 milliseconds between each number, you can use a closure to capture the current value of i for each iteration of the loop. One common way to achieve this is by using an Immediately Invoked Function

- Expression (IIFE) inside the loop. Here's how you can modify the code:


### Method 1:

```
  for (var i = 0; i < 10; i++) {
  (function (index) {
    setTimeout(() => {
      console.log(index);
    }, 100 * index); // Multiply delay by index to stagger the output
  })(i);
}
```

- This modification ensures that each setTimeout callback captures the value of i at the time of its creation, resulting in the expected output.


### Method 2:

```
for(let i=0; i< 10; i++){
  setTimeout(() => {
    console.log(i);
  }, 100)
}
```

### Output
0
1
2
3
4
5
6
7
8
9
