# Coin Change

Given a number between 1 and 99, return array which show how many quarters, dimes, nickels and pennies which make up the 'change'.


```javascript
/**
 * @param {number} change
 * @return {number}
 */
var coinChange = function(change) {
    let quarter = 25;
    let dime = 10;
    let nickel = 5;
    let penny = 1;
    let result = [0,0,0,0];

    // your code here.

    return result;
};
```

So if the function `coinChange` is given the following input, the function returns the output.

The output array is 
`[quarters, dimes, nickels, pennies]`

|Change input|Coins output|
|---|---|
|1|[0,0,0,1]|
|2|[0,0,0,2]|
|5|[0,0,1,0]|
|10|[0,1,0,0]|
|13|[0,1,0,3]|
|15|[0,1,1,0]|
|50|[2,0,0,0]|
|25|[1,0,0,0]|
|23|[0,2,0,3]|
|68|[2,1,1,3]|
|98|[3,4,0,3]|
|99|[3,4,0,4]|

Please note: If you have a choice of how to split the number, use the fewest coins. If for instance, the function get `50`, if should return 2 quarters - not 5 dimes, 10 nickels or 50 pennies.

#### A Solution

just one of many possible solutions.

```javascript
function coinChange(amt) {
    let carry = amt;
    let quarters = Math.floor(carry / 25);
    carry = carry % 25;
    let dimes = Math.floor(carry / 10);
    carry = carry % 10;
    let nickels = Math.floor(carry / 5);
    carry = carry % 5;
    let pennies = Math.floor(carry / 1);
    return [quarters, dimes, nickels, pennies];
}

console.log(0, coinChange(0));
console.log(1, coinChange(1));
console.log(13, coinChange(13));
console.log(23, coinChange(23));
console.log(98, coinChange(98));
console.log(99, coinChange(99));
```