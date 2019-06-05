# The Challange

https://www.codewars.com/kata/highest-and-lowest/train/javascript

```
In this little assignment you are given a string of space separated numbers, and have to return the highest and lowest number.

Example:

highAndLow("1 2 3 4 5");  // return "5 1"
highAndLow("1 2 -3 4 5"); // return "5 -3"
highAndLow("1 9 3 4 -5"); // return "9 -5"

Notes:

    All numbers are valid Int32, no need to validate them.
    There will always be at least one number in the input string.
    Output string must be two numbers separated by a single space, and highest number is first.
```

# My Answer

```
function highAndLow(numbers){
  var splitArray = numbers.split(" ");
  splitArray.sort(function(a, b){return a-b});
  return splitArray[splitArray.length-1] + " " + splitArray[0];
}
```

# Comments & Hurdles

* Previous code to sort and pick first and last items

# Favourite Answer (By Others)
```
function highAndLow(numbers){
  numbers = numbers.split(' ');
  return `${Math.max(...numbers)} ${Math.min(...numbers)}`;
}
```