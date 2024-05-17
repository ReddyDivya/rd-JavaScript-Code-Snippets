# Code Snippet - 19

```
myFun();
var myFun = function(){
  console.log("First");
}

myFun();

function myFun(){
  console.log("Second");
}
myFun();
```

# Code Explanation: 

- In the Memory Phase, `var myFun= undefined` since its a variable, later `function myFun(){console.log("Second");}` the copy of function is stored in the memory. 
- Later, in the Code Execution phase the first `myFun()` is pointing to `function myFun(){ console.log("Second"); }`. So, it prints `Second`. Then re-initialized with `First` for `var myFun = function(){
  console.log("First"); }`. So, for next two `myFun()`calls it logs `First`, `First`.
  
# Output
```
Second
First
First
```
