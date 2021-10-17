# 100 days of code, day 8

## Even numbers in an array

Given an array of digital numbers, return a new array of length number containing the last even numbers from the original array (in the same order). The original array will be not empty and will contain at least "number" even numbers.

For example:

```
([1, 2, 3, 4, 5, 6, 7, 8, 9], 3) => [4, 6, 8]
([-22, 5, 3, 11, 26, -6, -7, -8, -9, -8, 26], 2) => [-8, 26]
([6, -25, 3, 7, 5, 5, 7, -3, 23], 1) => [6]
```

```javascript
function evenNumbers(array, number) {
  var isEven = array.filter((n) => n % 2 === 0);
  return isEven.slice(-number);
}
```

---

## Finding the nth character in a string

```javascript
var name = Joseph;
var lastLetterOfName = name[name.length - 1];

console.log(lastLetterOfName); // output: h

var name = Joseph;
var lastLetterOfName = name[name.length - 3];

console.log(lastLetterOfName); // output: e
```

```javascript
var name = Joseph;
var firstLetterOfName = name[0];

console.log(firstLetterOfName); // output: J

var name = Joseph;
var firstLetterOfName = name[2];

console.log(firstLetterOfName); // output: o
```

---

## Tags

String intrapulation | Arrays | Basic language features | [freecodecamp.org](https://freecodecamp.org)
