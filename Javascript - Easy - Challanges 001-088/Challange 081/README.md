# The Challange

https://www.codewars.com/kata/exes-and-ohs/train/javascript

```
Check to see if a string has the same amount of 'x's and 'o's. The method must return a boolean and be case insensitive. The string can contain any char.

Examples input/output:

XO("ooxx") => true
XO("xooxx") => false
XO("ooxXm") => true
XO("zpzpzpp") => true // when no 'x' and 'o' is present should return true
XO("zzoo") => false
```

# My Answer

```
function XO(str) {
    var xCount = 0;
    var oCount = 0;
    
    for (var i = 0; i < str.length; i++){
      if (str[i].toLowerCase() == "o") {
        oCount += 1;
      } else if (str[i].toLowerCase() == "x") {
        xCount += 1;
      }
    }

    if (oCount == xCount){
      return true;
    } else {
      return false;
    }
}
```

# Comments & Hurdles

* loop, counter and check

# Favourite Answer (By Others)
```
function XO(str) {
  let x = str.match(/x/gi);
  let o = str.match(/o/gi);
  return (x && x.length) === (o && o.length);
}
```