# The Challange

https://www.codewars.com/kata/beginner-series-number-3-sum-of-numbers/train/javascript

```
Given two integers a and b, which can be positive or negative, find the sum of all the numbers between including them too and return it. If the two numbers are equal return a or b.

Note: a and b are not ordered!
Examples

GetSum(1, 0) == 1   // 1 + 0 = 1
GetSum(1, 2) == 3   // 1 + 2 = 3
GetSum(0, 1) == 1   // 0 + 1 = 1
GetSum(1, 1) == 1   // 1 Since both are same
GetSum(-1, 0) == -1 // -1 + 0 = -1
GetSum(-1, 2) == 2  // -1 + 0 + 1 + 2 = 2
```

# My Answer

```
function GetSum( a,b ) {

    if (a > b) {
        var startNumber = b;
        var endNumber = a;
    } else {
        var startNumber = a;
        var endNumber = b;
    }
    
    var totalCounter = 0;
    
    for (startNumber; startNumber <= endNumber; startNumber++){
        totalCounter += startNumber;
   }

   return totalCounter;
}
```

# Comments & Hurdles

* if statement made sure worked both ways but feel there's an cleaner way

# Favourite Answer (By Others)
```
const GetSum = (a, b) => {
  let min = Math.min(a, b),
      max = Math.max(a, b);
  return (max - min + 1) * (min + max) / 2;
}
```