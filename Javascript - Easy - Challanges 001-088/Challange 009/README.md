# The Challange

https://www.codewars.com/kata/counting-sheep-dot-dot-dot/train/javascript

```
Consider an array of sheep where some sheep may be missing from their place. We need a function that counts the number of sheep present in the array (true means present).

For example,

[true,  true,  true,  false,
  true,  true,  true,  true ,
  true,  false, true,  false,
  true,  false, false, true ,
  true,  true,  true,  true ,
  false, false, true,  true]

The correct answer would be 17.

Hint: Don't forget to check for bad values like null/undefined
```

# My Answer

```
function countSheeps(arrayOfSheep) {
  var sheepCounter = 0;
  
  for (var i = 0; i < arrayOfSheep.length; i++) {
      if (arrayOfSheep[i] === true) {
        sheepCounter += 1;
      }
    }
    return sheepCounter;
}
```

# Comments & Hurdles

* Looped through aray looking only for 'true'

# Favourite Answer (By Others)
```
function countSheeps(arrayOfSheeps) {
  return arrayOfSheeps.filter(Boolean).length;
}
```