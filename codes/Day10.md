# 100 days of code, day 10

## Stand in line

> In Computer Science a queue is an abstract Data Structure where items are kept in order. New items can be added at the back of the queue and old items are taken off from the front of the queue.

> > Write a function `nextInLine` which takes an array (`arr`) and a number (`item`) as arguments.
> > Add the number to the end of the array, then remove the first element of the array.
> > The `nextInLine` function should then return the element that was removed.

## Solution

```javascript
function nextInLine(arr, item) {
  // Only change code below this line
  arr.push(item);
  return arr.shift();
  // Only change code above this line
}

// Setup
var testArr = [1, 2, 3, 4, 5];

// Display code
console.log("Before: " + JSON.stringify(testArr)); // Before: [1,2,3,4,5]
console.log(nextInLine(testArr, 6)); // 1
console.log("After: " + JSON.stringify(testArr)); // After: [2,3,4,5,6]
console.log(nextInLine([5, 6, 7, 8, 9], 1)); // 5
console.log(nextInLine([2], 1)); // 2
```

## Tags

Array manipulation | Indexes | [freecodecamp.org](https://freecodecamp.org)
