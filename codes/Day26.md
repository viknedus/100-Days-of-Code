# 100 days of code, day 26

Create a two-dimensional array with `m` rows and `n` columns of zeroes.

> it should return a correct 3x2 array of zeroes, which looks like `[[0, 0], [0, 0], [0, 0]]`

## Solution

```javascript
function zeroArray(m, n) {
  // Creates a 2-D array with m rows and n columns of zeroes
  let newArray = [];

  // Adds the m-th row into newArray
  for (let i = 0; i < m; i++) {
    let row = [];

    for (let j = 0; j < n; j++) {
      // Pushes n zeroes into the current row to create the columns
      row.push(0);
    }
    // Pushes the current row, which now has n zeroes in it, to the array
    newArray.push(row);
  }
  return newArray;
}

let matrix = zeroArray(3, 2);
console.log(matrix); // [[0, 0], [0, 0], [0, 0]]
```

## Tag

Nested loop | for-loop | Array | Table | freecodecamp.org
