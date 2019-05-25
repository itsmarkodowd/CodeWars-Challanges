# The Challange

https://www.codewars.com/kata/opposite-number/train/javascript

```
Very simple, given a number, find its opposite.

Examples:

1: -1
14: -14
-34: 34
```

# My Answer

```
function opposite(number) {
  if (number > 0) {
    return -Math.abs(number);
  } else {
    return Math.abs(number);
  }
}
```

# Comments & Hurdles

* Googling came across Math.abs and -Math.abs for the answer
* The favourite answer took a way simpler approach

# Favourite Answer (By Others)
```
function opposite(number) {
  return(-number);
}
```