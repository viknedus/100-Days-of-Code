# 100 days of code, day 1

## Question

> Write a function that takes an integer as input, and returns the number of bits that are equal to one in the binary representation of that number. You can guarantee that input is non-negative.
>
> > Example: The binary representation of 1234 is 10011010010, so the function should return 5 in this case

---

## Solution

```javascript
var countBits = function (n) {
  return (result =
    n.toString(2).match(/1/g) != null ? n.toString(2).match(/1/g).length : 0);
};
```

---

### Tags
`Algorithms` | `bits` | `binary`
