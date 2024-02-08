# Code Snippet - 7

# Understanding Object References in JavaScript

```
let user = {name : "Virat Kohli"};
const userList = [user];
user = null; console.log(userList );
```

1/4: Objects in JavaScript are like containers for data. Picture creating a container called user labeled with name holding "Virat Kohli".

1/4: In JavaScript, objects are often passed by reference. Let's explore how this works with a simple example.

2/4: We start by creating an object user with a property name set to "Virat Kohli". We then create an array userList and store the user object in it.

3/4: Next, we set user to null. However, since objects are passed by reference, the userList array still holds a reference to the original user object.

4/4: As a result, when we log userList, it still contains the original user object. Understanding object references is crucial for managing data effectively in JavaScript! #JavaScript #ObjectReferences 🚀

## Output
```
[{ name: 'Virat Kohli' }]
```

This thread provides a clearer explanation of how objects and references work in JavaScript using a relatable analogy.

