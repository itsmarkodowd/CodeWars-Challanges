# The Challange

https://www.codewars.com/kata/exclamation-marks-series-number-1-remove-a-exclamation-mark-from-the-end-of-string/train/javascript
```
 Remove a exclamation mark from the end of string. For a beginner kata, you can assume that the input data is always a string, no need to verify it.
Examples

remove("Hi!") === "Hi"
remove("Hi!!!") === "Hi!!"
remove("!Hi") === "!Hi"
remove("!Hi!") === "!Hi"
remove("Hi! Hi!") === "Hi! Hi"
remove("Hi") === "Hi"
```

# My Answer

```
function remove(s){
  if (s[s.length - 1] == '!'){
    return s.slice(0, s.length - 1);
  } else {
    return s;
  }
}
```

# Comments & Hurdles

* if() check if last index is !
* slice() if it is
* fav - regex check was clever

# Favourite Answer (By Others)
```
const remove = s => s.replace(/!$/, '');
```