# The Challange

https://www.codewars.com/kata/calculate-average/train/javascript

```
Write function avg which calculates average of numbers in given list.

```

# My Answer

```
function find_average(array) {
  var total = 0;
  for (var i = 0; i < array.length; i++) {
    total += array[i];
  }
  return (total / array.length);
}
```

# Comments & Hurdles

* Straightforward
* I need to look into reduce() more

# Favourite Answer (By Others)
```
function find_average(array) {
  var sum = array.reduce((a, b) => a + b, 0);
  return sum/array.length;
}
```