# String to Integer

Convert a string of a number to a number.
The input will always be a positive number with no decimal places.

So valid input is:
```
"1"
"4"
"16"
"50634"
```
but valid input is __not__ 
```
"-7"
"0.5"
"134.006"
```

```javascript
/**
 * @param {string} s
 * @return {number}
 */
var myAtoi = function(s) {
    return 0;
};
```

### Example 1

```
let s = "42"
let i = myAtoi(s)
```
output: i = 42

### Example 2

```
let s = "1456"
let i = myAtoi(s)
```
output: i = 1456


### Example 3

```javascript
let s = "672"
let i = myAtoi(s)
```

output: i = 672

### One Solution

```javascript
let input1 = "1234";
// output should be
output1 = 1234;

function myAtoi(s) {
    let result = 0;
    let nsl = s.split("").reverse();
    for (let i = nsl.length-1; i >= 0; i--) {
        result += parseInt(nsl[i], 10) * Math.pow(10, i);
    }
    return result;
}

console.log(myAtoi(input1));
console.log(myAtoi("4567"));
console.log(myAtoi("17"));
console.log(myAtoi("7"));
```
