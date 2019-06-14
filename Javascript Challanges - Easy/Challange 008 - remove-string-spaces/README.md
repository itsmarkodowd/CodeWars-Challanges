# The Challange

https://www.codewars.com/kata/remove-string-spaces/train/javascript

```
Simple, remove the spaces from the string, then return the resultant string.
```

# My Answer

```
function noSpace(x){
  return x.split(' ').join('');
}
```

# Comments & Hurdles

* split(' ') mixed with join('') worked perfect
* apparently faster than regex method

# Favourite Answer (By Others)
```
const noSpace = (str) => str.replace(/\s*/g, '');
```