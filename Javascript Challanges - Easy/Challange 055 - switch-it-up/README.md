# The Challange

https://www.codewars.com/kata/switch-it-up/train/javascript
```
When provided with a number between 0-9, return it in words.

Input :: 1

Output :: "One".

Try using "Switch" statements.
```

# My Answer

```
function switchItUp(number){

  switch (number) {
    case 0:
      return "Zero";
      break;
    case 1:
      return "One";
      break;
    case 2:
       return "Two";
      break;
    case 3:
      return "Three";
      break;
    case 4:
      return "Four";
      break;
    case 5:
      return "Five";
      break;
    case 6:
      return "Six";
      break;
    case 7:
      return "Seven";
      break;
    case 8:
      return "Eight";
      break;
    case 9:
      return "Nine";
  }
}
```

# Comments & Hurdles

* Challange requested switch statement
* I didn't need to "break" return did that already

# Favourite Answer (By Others)
```
function switchItUp(number) {
  switch (number) {
    case 0: return 'Zero';
    case 1: return 'One';
    case 2: return 'Two';
    case 3: return 'Three';
    case 4: return 'Four';
    case 5: return 'Five';
    case 6: return 'Six';
    case 7: return 'Seven';
    case 8: return 'Eight';
    case 9: return 'Nine';
  }
}
```