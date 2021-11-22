# 100 days of code, day 27

## Basic data structures

> Iterate Through All an Array's Items Using For Loops

Using a For-loop, to return a filtered version of the passed array such that any array nested within `arr` containing `elem` has been removed.

## Solution

```javascript
function filteredArray(arr, elem) {
  let newArr = [];

  for (let i = 0; i < arr.length; i++) {
    // Checks every parameter for the element and if is NOT there continues the code
    if (arr[i].indexOf(elem) == -1) {
      //Inserts the element of the array in the new filtered array
      newArr.push(arr[i]);
    }
  }

  return newArr;
}

console.log(
  filteredArray(
    [
      [3, 2, 3],
      [1, 6, 3],
      [3, 13, 26],
      [19, 3, 9],
    ],
    3
  )
); // []
```

## Possible outcomes

- `filteredArray([[3, 2, 3], [1, 6, 3], [3, 13, 26], [19, 3, 9]], 3)` should return `[]`
- `filteredArray([[10, 8, 3], [14, 6, 23], [3, 18, 6]], 18)` should return `[[10, 8, 3], [14, 6, 23]]`
- `filteredArray([["trumpets", 2], ["flutes", 4], ["saxophones", 2]], 2)` should return `[["flutes", 4]]`
- `filteredArray([["amy", "beth", "sam"], ["dave", "sean", "peter"]], "peter")` should return `[["amy", "beth", "sam"]]`

## Tag

Nested Array | For-loop | indexOf() | freecodecamp.org
