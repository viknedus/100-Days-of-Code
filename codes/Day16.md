# 100 days of code, day 16

## Nesting for-loops

Given an array of integers, return the product of the array values usinf for-loop.

**Example:** `multiplyAll([[1,2],[3,4],[5,6,7]])` should return `5040`

```javascript
function multiplyAll(arr) {
  var product = 1;
  for (var i = 0; i < arr.length; i++) {
    for (var j = 0; j < arr[i].length; j++) {
      product *= arr[i][j];
    }
  }
  return product;
}

multiplyAll([
  [1, 2],
  [3, 4],
  [5, 6, 7],
]);
```
## Tag
for-loop | Arrays | [Freecodecamp](https://freecodecamp.com)