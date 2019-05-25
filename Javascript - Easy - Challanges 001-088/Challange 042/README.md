# The Challange

https://www.codewars.com/kata/to-square-root-or-not-to-square-root/train/javascript

```
Write a method, that will get an integer array as parameter and will process every number from this array.
Return a new array with processing every number of the input-array like this:

If the number has an integer square root, take this, otherwise square the number.

[4,3,9,7,2,1] -> [2,9,3,49,4,1]
```

# My Answer

```
function squareOrSquareRoot(array) {

function myFunction(value) {
  if (value % Math.sqrt(value) == 0) {
    return Math.sqrt(value);
  } else {
    return value ** 2;
  }
}

  return array.map(myFunction);
};
```

# Comments & Hurdles

* map() good iterator but my if statement seems convoluted

# Favourite Answer (By Others)
```
function squareOrSquareRoot(array) {
  return array.map(x => {
    const r = Math.sqrt(x);
    return (r % 1 == 0) ? r : (x*x);
  });  
}
```