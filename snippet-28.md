const name = "john"; // Declaring a constant `name` with value "john".
const age = 3;       // Declaring a constant `age` with value 3.

// Using object shorthand to create an object `person`.
// Instead of writing {name: name, age: age}, you can just write {name, age}.
const person = {name, age, subject: "js"};

console.log("person-", person);
// Output: person- { name: 'john', age: 3, subject: 'js' }
// The `person` object includes the properties `name`, `age`, and `subject`.

// Logs the individual variables `name` and `age`.
console.log("", name, age);
// Output:  john 3
// The values of `name` and `age` are displayed as separate arguments.

// Demonstrating object shorthand again.
console.log("object shorthand - ", {name, age});
// Output: object shorthand -  { name: 'john', age: 3 }
// This creates a new object inline with properties `name` and `age` using shorthand syntax.
