# 100 days of code, day 21

## Destructuring Assignment with the Rest Parameter to Reassign Array Elements

Use destructuring assignment with the rest parameter to perform an effective `Array.prototype.slice()` so that `arr` is a sub-array of the original array `source` with the first two elements omitted.

```javascript
const source = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
function removeFirstTwo(list) {
  "use strict";
  const [a, b, ...arr] = list;
  return arr;
}

const arr = removeFirstTwo(source);

console.log(arr); // should be [3,4,5,6,7,8,9,10]
console.log(source); // should be [1,2,3,4,5,6,7,8,9,10];
```

- Destructuring on `list` will be used.
- Array.slice() is not used.

## Tag

Destructuring | Arrays | spread operator | [freecodecamp.com](https://freecodecamp.com)
