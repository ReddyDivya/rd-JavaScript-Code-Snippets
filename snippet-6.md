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

- 1/4: Ever used setTimeout inside a loop in JavaScript? Let's explore a common pitfall with this code snippet:

- 2/4: for(var i=0; i<10; i++){ setTimeout(() => {console.log(i)}, 8)}. It logs values of i after a delay using setTimeout.

- 3/4: Due to JavaScript's asynchronous nature, all logs print the final value of i, 10, instead of 0 to 9.

## Output
```
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
```

- 4/4: Fixing the issue is simple: replace var with let in the loop declaration. This ensures each setTimeout captures the correct i value.

```
for(let i=0; i<10; i++)
{
  setTimeout(() => {
    console.log(i)
  }, 8);
}
```
## Output
```
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
```

Understanding this helps write robust JavaScript! #JavaScript #Programming 🚀
