# Code Snippet - 14

```
let user = {name: "Virat Kohli"};
let userlist = [user];
user = null;

console.log(userlist);//(1) [{...}]
console.log(user);//null
```

# Output
```
(1) [{...}]
null
```

# Code Explanation:
Let's break down the code step by step:

```
let user = {name: "Virat Kohli"};
```
- This line declares a variable user and initializes it with an object {name: "Virat Kohli"}. This object has a property name with the value "Virat Kohli".

```
let userlist = [user];
```
- Here, an array userlist is declared and initialized with a single element, which is the user object. This means userlist contains a reference to the same object that user is referencing.

```
user = null;
```
- This line assigns the value null to the variable user. This does not affect the array userlist because userlist contains a reference to the original object, not to the user variable itself.

```
console.log(userlist);
```

- Finally, console.log(userlist) prints the content of the userlist array to the console.
- Since the user object was not directly modified, but rather the variable user was reassigned to null, the reference to the original object in userlist remains unchanged.
- Therefore, userlist still contains a reference to the {name: "Virat Kohli"} object, and the output will be an array with one element, which is the {name: "Virat Kohli"} object.
