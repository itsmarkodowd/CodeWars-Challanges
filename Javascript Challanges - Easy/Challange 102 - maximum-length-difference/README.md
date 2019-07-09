# The Challange

https://www.codewars.com/kata/maximum-length-difference/train/javascript

```
You are given two arrays a1 and a2 of strings. Each string is composed with letters from a to z. Let x be any string in the first array and y be any string in the second array.

Find max(abs(length(x) − length(y)))

If a1 and/or a2 are empty return -1 in each language except in Haskell (F#) where you will return Nothing (None).

#Example:

a1 = ["hoqq", "bbllkw", "oox", "ejjuyyy", "plmiis", "xxxzgpsssa", "xxwwkktt", "znnnnfqknaz", "qqquuhii", "dvvvwz"]
a2 = ["cccooommaaqqoxii", "gggqaffhhh", "tttoowwwmmww"]
mxdiflg(a1, a2) --> 13
```

# My Answer

```
function mxdiflg(a1, a2) {

  if (a1.length == 0 || a2.length == 0) {
   return -1;
  }
  
  let a1Sort = a1.sort((a, b) => b.length - a.length);
  let a2Sort = a2.sort((a, b) => b.length - a.length);
  
  let longestA1 = a1Sort[0].length;
  let longestA2 = a2Sort[0].length;
  
  let shortestA1 = a1Sort[a1Sort.length - 1].length;
  let shortestA2 = a2Sort[a2Sort.length - 1].length;
  
  return Math.max(Math.abs(longestA1 - shortestA2), Math.abs(longestA2 - shortestA1));
}
```

# Comments & Hurdles

* Made a complete mess and don't like my answer
* The question I thought was badly asked
* Fav - This answer was so clear to understand

# Favourite Answer (By Others)
```
function mxdiflg(a1, a2) {
  if (a1.length === 0 || a2.length === 0) return -1
  let l1 = a1.map(str => str.length)
  let l2 = a2.map(str => str.length)
  return Math.max(Math.max(...l1) - Math.min(...l2), Math.max(...l2) - Math.min(...l1))
}
```