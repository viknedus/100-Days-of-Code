# 100 days of code, day 28

## Basic data structures

> Iterate Through the Keys of an Object with a for...in Statement

Function `countOnline` which accepts one argument (a users object). Use a for...in statement within this function to loop through the users object passed into the function and return the number of users whose `online` property is set to `true`. An example of a users object which could be passed to `countOnline` is shown below. Each user will have an online property with either a `true` or `false` value

```javascript
let users = {
  Alan: {
    online: false,
  },
  Jeff: {
    online: true,
  },
  Sarah: {
    online: false,
  },
};
```

## Proposed solution

```javascript
function countOnline(usersObj) {
  let result = 0;
  for (let user in usersObj) {
    if (usersObj[user].online === true) {
      result++;
    }
  }
  return result;
}

console.log(countOnline(users)); // 1
```

## Proposed outcomes

- The function countOnline should return `1` when the object `{ Alan: { online: false }, Jeff: { online: true }, Sarah: { online: false } }` is passed to it
- The function countOnline should return `2` when the object `{ Alan: { online: true }, Jeff: { online: false }, Sarah: { online: true } }` is passed to it
- The function countOnline should return `0` when the object `{ Alan: { online: false }, Jeff: { online: false }, Sarah: { online: false } }` is passed to it

## Tag

For-in Loop | Arrays | freecodecamp.org
