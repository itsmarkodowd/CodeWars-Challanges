# The Challange

https://www.codewars.com/kata/removing-elements/train/javascript
```
Take an array and remove every second element out of that array. Always keep the first element and start removing with the next element.

Example:

myArr = ['Keep', 'Remove', 'Keep', 'Remove', 'Keep', ...];
```

# My Answer

```
function removeEveryOther(arr){
  let newArr = []
  
  for (let i = 0; i < arr.length; i += 2){
    newArr.push(arr[i]);
  }
  return newArr;
}
```

# Comments & Hurdles

* For loop with +=2 at end
* Filter iterator harder to read

# Favourite Answer (By Others)
```
function removeEveryOther(arr){
  return arr.filter(function(elem, index) {
    return index % 2 === 0;
  });
}
```