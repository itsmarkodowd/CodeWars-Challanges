# The Challange

https://www.codewars.com/kata/total-amount-of-points/train/javascript

```
Our football team finished the championship. The result of each match look like "x:y". Results of all matches are recorded in the collection.

For example: ["3:1", "2:2", "0:1", ...]

Write a function that takes such collection and counts the points of our team in the championship. Rules for counting points for each match:

    if x>y - 3 points
    if x<y - 0 point
    if x=y - 1 point
```

# My Answer

```
function points(games) {

let total = 0;

for (let i = 0; i < games.length; i++){
  if (games[i][0] > games[i][2]){
    total += 3;
  } else if (games[i][0] == games[i][2]){
    total += 1;
}  else {
    total += 0;
    }
}
    return total;
}
```

# Comments & Hurdles

* My code feels messy
* Need to focus on learning array iterators

# Favourite Answer (By Others)
```
const points = a => a.reduce((r, e) => {
  const x = e[0];
  const y = e[2];
  return r + (x > y ? 3 : x < y ? 0 : 1);
}, 0);
```

# Favourite Analysed

* reduce() method runs a function on each array element to produce (reduce it to) a single value.
* Assigned the value of each index (e[0]) and (e[2]) as const to be compared
* return fuction adds a value to the total tally (r) based on Conditional (Ternary) Operator (?). +3 if greater, +0 if less and +1 otherwise (tie)