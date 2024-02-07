# Code Snippet - 4:

```
console.log(parseInt("18"));//18
console.log(parseInt("101*3"));//101
console.log(parseInt("81javascript-code"));//81
```

## Explanation:
- `console.log(parseInt("18"));//18`: This line converts the string "18" to an integer using parseInt. Since "18" contains a valid integer representation, it returns the integer 18, which is then logged to the console.
- `console.log(parseInt("101*3"));//101`: Here, parseInt parses the string "101*3". It stops parsing at the non-numeric character "*", so it converts "101" to the integer 101, which is then logged to the console.
- `console.log(parseInt("81javascript-code"));//81`: Similarly, parseInt parses the string "81javascript-code". It stops parsing at the non-numeric character "j", so it converts "81" to the integer 81, which is then logged to the console.

## Output
```
18
101
81
```

In summary, parseInt extracts an integer from the beginning of a string until it encounters a non-numeric character. It returns the parsed integer or NaN if the string doesn't start with a valid numeric representation.

---

Simple Thread on JavaScript's parseInt() 🧵

1/4: The code snippet console.log(parseInt("18"));//18 converts the string "18" to an integer, giving us 18. This is straightforward as "18" represents a valid integer.

2/4: In console.log(parseInt("101*3"));//101, parseInt() stops parsing at the non-numeric character "*" and returns the integer 101. It extracts the numeric part of the string until it reaches a non-numeric character.

3/4: Similarly, console.log(parseInt("81javascript-code"));//81 extracts the numeric part "81" from the string and returns the integer 81. It ignores the non-numeric characters ("javascript-code") after the number.

4/4: Summary: parseInt() in JavaScript parses strings to integers. It stops parsing when it encounters a non-numeric character and returns the extracted integer. Understanding this behavior is key for proper string-to-integer conversions in JavaScript. #JavaScript #parseInt #Programming 🚀

---

