# The Challange

https://www.codewars.com/kata/counting-duplicates/train/javascript

```
Count the number of Duplicates

Write a function that will return the count of distinct case-insensitive alphabetic characters and numeric digits that occur more than once in the input string. The input string can be assumed to contain only alphabets (both uppercase and lowercase) and numeric digits.
Example

"abcde" -> 0 # no characters repeats more than once
"aabbcde" -> 2 # 'a' and 'b'
"aabBcde" -> 2 # 'a' occurs twice and 'b' twice (`b` and `B`)
"indivisibility" -> 1 # 'i' occurs six times
"Indivisibilities" -> 2 # 'i' occurs seven times and 's' occurs twice
"aA11" -> 2 # 'a' and '1'
"ABBA" -> 2 # 'A' and 'B' each occur twice
```

# My Answer

```
function duplicateCount(text){
  let obj = {};
  let textLower = text.toLowerCase();
  let counter = 0;

  //Each letter added to object
  for (i = 0; i < text.length; i++){
    obj[textLower[i]] = 0;
  };
  
  //Tally each letter to object
  for (i = 0; i < text.length; i++){
    if (obj.hasOwnProperty(`${textLower[i]}`)){
      obj[textLower[i]] += 1;
    }
  };
  
  //Check how many letters > 1 and tally  
  for (i = 0; i < Object.keys(obj).length; i++){
    if (obj[Object.keys(obj)[i]] > 1) {
      counter += 1;
    }
  }
  
  return counter;
}
```

# Comments & Hurdles

* Last loop over object felt messy
* I should have converted into array to get ideas
* Fav - comparing indexOf and lastIndexOf much simpler
* Fav - could even be cleaned up a little for more clarity (=>)


# Favourite Answer (By Others)
```
function duplicateCount(text){
  return text.toLowerCase().split('').filter(function(val, i, arr){
    return arr.indexOf(val) !== i && arr.lastIndexOf(val) === i;
  }).length;
}
```