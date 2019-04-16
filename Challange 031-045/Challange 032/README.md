# The Challange

https://www.codewars.com/kata/vowel-count/train/javascript

```
Return the number (count) of vowels in the given string.

We will consider a, e, i, o, and u as vowels for this Kata.

The input string will only consist of lower case letters and/or spaces.

```

# My Answer

Passed all tests and found inside script.js

# Comments & Hurdles

* Just multiple || comparrisons in if statement

# Favourite Answer (By Others)
```
function getCount(str) {
  return (str.match(/[aeiou]/ig)||[]).length;
}
```