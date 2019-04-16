# The Challange

https://www.codewars.com/kata/remove-string-spaces/train/javascript

```
Simple, remove the spaces from the string, then return the resultant string.
```

# My Answer

Passed all tests and found inside script.js

# Comments & Hurdles

* split(' ') mixed with join('') worked perfect
* apparently faster than regex method

# Favourite Answer (By Others)
```
const noSpace = (str) => str.replace(/\s*/g, '');
```