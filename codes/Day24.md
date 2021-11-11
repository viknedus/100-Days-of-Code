# 100 days of code, day 24

## Template Literal

Use template literal syntax with backticks to create an array of list element (`li`) strings. Each list element's text should be one of the array elements from the `failure` property on the `result` object and have a `class` attribute with the value `text-warning`. The `makeList` function should return the array of list item strings.

_Of cause there are more better efficient ways to achieve this result but the above instructions will be followed_

_Use an iterator method (any kind of loop) to get the desired output (shown below)_

```javascript
[
  '<li class="text-warning">no-var</li>',
  '<li class="text-warning">var-on-top</li>',
  '<li class="text-warning">linebreak</li>',
];
```

### Solution

```javascript
// run `node index.js` in the terminal

const result = {
  success: ["max-length", "no-amd", "prefer-arrow-functions"],
  failure: ["no-var", "var-on-top", "linebreak"],
  skipped: ["no-extra-semi", "no-dup-keys"],
};
function makeList(arr) {
  // Using for-loop
  const failureItems = [];
  for (let i = 0; i < arr.length; i++) {
    failureItems.push(`<li class="text-warning">${arr[i]}</li>`);
  }

  // Or .map()
  // const failureItems = arr.map(item => `<li class="text-warning">${item}</li>`);

  return failureItems;
}

const failuresList = makeList(result.failure);

console.log(failuresList); // will produce above desired solution
```

## Tag

Template literal | Strings | for-loop | map() | Arrays | freecodecamp.com
