# Code snippet - 11

```
console.log(parseInt("108"));//108
console.log(parseInt("2*108"));//2
console.log(parseInt("8wonders"));//8
```

# Code Explanation:

`console.log(parseInt("108"));`
- This code uses the parseInt() function to parse the string "108" as an integer.
- Since "108" is a valid representation of an integer, it converts the entire string to an integer without any issue.
- Output: 108

`console.log(parseInt("2*108"));`
- This code attempts to parse the string "2*108" as an integer using the parseInt() function.
- The parseInt() function starts parsing from the beginning of the string until it encounters a character that is not a valid part of a number.
- In this case, it stops parsing at the character *, which is not a valid part of a number.
- So, only the substring "2" is successfully parsed as an integer, and the rest of the string ("*108") is ignored.
- Output: 2

`console.log(parseInt("8wonders"));`
- This code tries to parse the string "8wonders" as an integer using the parseInt() function.
- The parseInt() function starts parsing from the beginning of the string until it encounters a character that is not a valid part of a number.
- It stops parsing at the character w, which is not a valid part of a number.
- So, only the substring "8" is successfully parsed as an integer, and the rest of the string ("wonders") is ignored.
- Output: 8

In summary, the parseInt() function attempts to parse a string as an integer, but it stops parsing as soon as it encounters a character that is not part of a number. If the string starts with a valid numeric representation, it will be parsed as an integer. Otherwise, it will return NaN (Not a Number).
