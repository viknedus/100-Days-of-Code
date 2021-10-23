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

---

## Profile look-up

We have an array of objects representing different people in our contacts lists.

A `lookUpProfile` function that takes `name` and a property (`prop`) as arguments has been pre-written for you.

The function should check if `name` is an actual contact's `firstName` and the given property (`prop`) is a property of that contact.

If both are true, then return the "value" of that property.

If `name` does not correspond to any contacts then return the string `No such contact`.

If `prop` does not correspond to any valid properties of a contact found to match `name` then return the string `No such property`.

## Proposed solution

```javascript
var contacts = [
  {
    firstName: "Akira",
    lastName: "Laine",
    number: "0543236543",
    likes: ["Pizza", "Coding", "Brownie Points"],
  },
  {
    firstName: "Harry",
    lastName: "Potter",
    number: "0994372684",
    likes: ["Hogwarts", "Magic", "Hagrid"],
  },
  {
    firstName: "Sherlock",
    lastName: "Holmes",
    number: "0487345643",
    likes: ["Intriguing Cases", "Violin"],
  },
  {
    firstName: "Kristian",
    lastName: "Vos",
    number: "unknown",
    likes: ["JavaScript", "Gaming", "Foxes"],
  },
];

function lookUpProfile(name, prop) {
  for (let i = 0; i < contacts.length; i++) {
    if (contacts[i].firstName === name) {
      // if (contacts[i].hasOwnProperty(prop)){}
      if (prop in contacts[i]) {
        return contacts[i][prop];
      } else {
        return "No such property";
      }
    }
  }
  return "No such contact";
}

lookUpProfile("Akira", "likes"); // output: ["Pizza", "Coding", "Brownie Points"]
```

## Possible outcomes

- `lookUpProfile("Kristian", "lastName"`) should return the string `Vos`
- `lookUpProfile("Sherlock", "likes")` should return `["Intriguing Cases", "Violin"]`
- `lookUpProfile("Harry", "likes")` should return an `["Hogwarts", "Magic", "Hagrid"]`
- `lookUpProfile("Bob", "number")` should return the string `No such contact`
- `lookUpProfile("Akira", "address")` should return the string `No such property`.

## Tag

for-loop | if-else statement | Objects | Arrays | [Freecodecamp](https://freecodecamp.com)
