# Array Element Change - (10 pts)

You can change the values of an array.

`arr = [1,2,3,4,5,6]`

Create some code where the following happen.

- make the last element of the array equal to `11`
- make the first element equal to `8`
- make the second element equal to the sum of the last and first element
- zero out the fourth element

When you are finished, the array should be:

`arr = [8,19,3,4,0,11]`

### How to Solve

You can change any element in the array.
You need to use `indexes` in an array, BUT the array indexes go from `0` to `arr.length-1`.

```javascript
// the array places are named
       0 1 2 3 4 5
arr = [6,7,4,2,8,3];
```

So if you wanted to change the third item, you have to change `arr[2]` !
That's because the first element in an array is *always* `arr[0]`. (So, yes, it can be confusing to describe the first element as having a zero index.) (So much so that sometimes coders refer to that element as the _zeroth_ element.)

In Javascript, an array *always* has a _length_ property.
`let l = arr.length;` and in this case, `l` would end up being 6 (with the elements numbered from 0 to 5).

Remember, the index of the )last element_ in a javascript array is _always_ the length - 1.
