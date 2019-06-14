# The Challange

https://www.codewars.com/kata/reversed-strings/train/javascript

```
Complete the solution so that it reverses the string value passed into it.

solution('world'); // returns 'dlrow'
```

# My Answer

```
function solution(str){
    return str.split("").reverse().join("");
}
```

# Comments & Hurdles

* Had to combine the 3 built-in functions

# Favourite Answer (By Others)
```
const solution = str => str.split('').reverse().join('');
```