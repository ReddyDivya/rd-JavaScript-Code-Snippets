# Code Snippet - 5

# Simple Thread on Deleting JavaScript Variables 🧵

```
const name = 'Prabhas';
age = 44;
console.log(delete name); 
console.log(delete age);
```

# Explanation:

## delete operator

1/4: In JavaScript, we have the delete operator to remove properties from objects. But did you know it behaves differently with variables?

2/4: Let's break it down. `const name = 'Prabhas';` declares a constant variable name with the value 'Prabhas'. It cannot be deleted using delete.

3/4: On the other hand, age = 44; assigns 44 to an undeclared variable age, which becomes a property of the global object (e.g., window in browser environments). This property can be deleted using the delete operator.

4/4: `console.log(delete name);//false` logs false, indicating failure to delete name, while `console.log(delete age);//true` logs true, successfully deleting age. 

## Output
```
false
true
```

Understanding how delete works with variables is crucial in JavaScript! #JavaScript #Programming #javascript🚀
