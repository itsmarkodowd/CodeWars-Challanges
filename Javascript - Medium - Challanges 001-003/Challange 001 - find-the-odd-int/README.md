# The Challange

https://www.codewars.com/kata/find-the-odd-int/train/javascript

```
Given an array, find the int that appears an odd number of times.

There will always be only one integer that appears an odd number of times.

```

# My Answer

```
function findOdd(A) {
  var objCounter = {};

//Filling objCounter
  for (var i = 0; i < A.length; i++) {
    if (objCounter[A[i]] == true){
      objCounter[A[i]]++;
    } else {
      objCounter[A[i]] = 1;
    }
  }

//Checking objCounter
  for (var key in objCounter) {
    if (objCounter[key] % 2 !== 0) {
      return Number(key);
    }
  }
};
```

# Comments & Hurdles

* Difficulty definetly increased
* Used an object to store number as a key and its value as a counter
* Two loops - first to fill then second to search for the odd value
* Favourite answer could take some reading up on reduce() and bitwise (^)

# Favourite Answer (By Others)
```
function findOdd(A) {
  return A.reduce(function(c,v){return c^v;},0);
}
```