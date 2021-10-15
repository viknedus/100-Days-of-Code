# 100 days of code, day 9

## Modifying Arrays with Indexes

```javascript
var myData = [10, 25, 30];
myData[1] = 20;

console.log(myData); // output: [10, 20, 30]
```

## Access multi-dimentional Arrays with Indexes

```javascript
var arr = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9],
  [[10, 11, 12], 13, 14],
];

console.log(arr[3]); // output: [[10, 11, 12], 13, 14]
console.log(arr[3][0]); // output: [10, 11, 12]
console.log(arr[3][0][1]); // output: 11
```

## Manipulate Arrays with pop(), shift(), unshift() and push()

```javascript
/* pop() removes last value in an array */
var threeArr = [1, 4, 6];
var oneDown = threeArr.pop();

console.log(threeArr); // output: [1, 4]
console.log(oneDown); // output: 6
```

```javascript
/* shift() removes first value in an array */
var threeArr = [1, 4, 6];
var oneDown = threeArr.shift();

console.log(threeArr); // output: [4, 6]
console.log(oneDown); // output: 1
```

```javascript
/* unshift() adds new value in the begining of an array */
var threeArr = [1, 4, 6];
var oneDown = threeArr.shift();
var oneUp = threeArr.unshift(3); // unshift()

console.log(threeArr); // output: [4, 6]
console.log(oneDown); // output: 1
console.log(oneUp); // output: [3, 4, 6]
```

```javascript
/* push() adds new value in the end of an array */
var arr1 = [1, 2, 3];
arr1.push(4); // output: [1,2,3,4]

var arr2 = ["Stimpson", "J", "cat"];
arr2.push(["happy", "joy"]); // output: ["Stimpson", "J", "cat", ["happy", "joy"]]
```

## Tags

Array manipulation | Indexes | [freecodecamp.org](https://freecodecamp.org)
