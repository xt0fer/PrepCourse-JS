# Last and First - Easy (50 pts)

Given a string, return a new string made up of its last and first letters, reversed and separated by a space.
Write it as a function

```js

function firstAndLast(s) {
    return "";
}
```

### Example

Given the string 'school', return the string 'l s'. 

### Function Description

Complete the function `lastFirstLetters` in the editor below. `lastFirstLetters` has the following parameter(s):

- string word: a string to process Returns:
- string: a string of two space-separated characters 

### Constraint

2 ≤ length of word ≤ 100

### Input Format for Custom Testing

Input from stdin will be processed as follows and passed to the function.
The line contains a string, word. 

### Sample Case 0

_Sample Input_ `APPLE`

_Sample Output_ `E A`

### Explanation

The last letter in 'APPLE' is E and the first letter is A, so return `E A`.


### Sample Case 1

_Sample Input_ `Orange`

_Sample Output_ `e O`

### Explanation

The last letter in 'Orange' is e and the first letter is O, so return `e O`.

### Sample Case 2

_Sample Input_ `bus`

_Sample Output_ `s b`

### Explanation

The last letter in 'bus' is s and the first letter is b, so return `s b`.
