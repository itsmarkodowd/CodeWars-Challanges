# The Challange

https://www.codewars.com/kata/odd-or-even/train/javascript

```
Given an array of numbers (a list in groovy), determine whether the sum of all of the numbers is odd or even.

Give your answer in string format as 'odd' or 'even'.

If the input array is empty consider it as: [0] (array with a zero).
```

# My Answer

```
const oddOrEven = array => (array.length == 0 ? 'even' : array.reduce((acc, val) => acc + val) % 2 == 0) ? 'even' : 'odd';
```

# Comments & Hurdles

* Wanted to make it 1 line so had to use 2 ternary
* Fav - using 0 as second argument of reduce would have simplified my answer

# Favourite Answer (By Others)
```
function oddOrEven(arr) {
  return arr.reduce((a,b)=>a+b,0) % 2 ? 'odd' : 'even';
}
```