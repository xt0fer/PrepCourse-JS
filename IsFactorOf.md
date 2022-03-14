# Is Factor Of - (20 pts)

Given two numbers `num` and `f`, returns `true` if `f` is a factor of `num`.

### Example

If the function is given the following inputs, see various results:

|num|f|result|
|---|---|---|
|6|2|true|
|4|2|true|
|3|2|false|
|10|2|true|
|5|2|false|
|16|4|true|
|15|4|false|

### Function Description

Complete the function `isFactorOf` in the editor below. `isFactorOf` has the following parameter(s):

- number num: number to test 
- number f: factor number 

Returns:
- true or false: depending on inputs 

```javascript
function isFactorOf(num, f) {
    return false;
}
```

### Explanation

Using `modulo` or `remainder` to decide if something is a factor or not. Check out how the `%` operator works.
If the `remainder` of a division is zero, then the numbers are factors.

- 6 % 2 = 0
- 4 % 2 = 0
- 3 % 2 = 1
- 10 % 2 = 0
- 5 % 2 = 1
- 16 % 4 = 0
- 15 % 4 = 3
- 14 % 4 = 2
- 13 % 4 = 1

Obviously, you can use the `%` to decide whether or not `f` is a factor of `num`.

If `num % f` results in a `0` value, then return `true`. Otherwise return `false`.