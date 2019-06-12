# The Challange

https://www.codewars.com/kata/simple-multiplication/train/javascript
```
This kata is about multiplying a given number by eight if it is an even number and by nine otherwise.
```

# My Answer

```
const simpleMultiplication = (num) => (num % 2 == 0) ? (num * 8) : (num * 9);
```

# Comments & Hurdles

* Used arrow function
* Used ternary operator (?)

# Favourite Answer (By Others)
```
function simpleMultiplication(n) {
    return n * (n % 2 ? 9 : 8);
}
```