# The Challange

https://www.codewars.com/kata/can-we-divide-it/train/javascript

```
Your task is to create functionisDivideBy (or is_divide_by) to check if an integer number is divisible by each out of two arguments.
```

# My Answer

```
const isDivideBy = (number, a, b) => (Math.abs(number) % Math.abs(a) == 0 && Math.abs(number) % Math.abs(b) == 0) ? true : false;
```

# Comments & Hurdles

* Using Math.abs() on everything seemed inefficent
* Fav - apparently didn't need Math.abs() or the Ternary Operator

# Favourite Answer (By Others)
```
const isDivideBy = (number, a, b) => number % a === 0 && number % b === 0;
```