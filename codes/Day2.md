# 100 days of code, day 2

## Question 1

> Complete the square sum function so that it squares each number passed into it and then sums the results together.
>
> > For example, for [1, 2, 2] it should return 9 because 1^2 + 2^2 + 2^2 = 9.

---

## Solution 1

```javascript
function squareSum(numbers) {
  return numbers.reduce((a, b) => a + Math.pow(b, 2), 0);
}
```

I used `reducer` and `Math.pow()` to find the solution

---

## Question 2

> Given an array of integers as strings and numbers, return the sum of the array values as if all were numbers.
>
> > For example, for [9, '3', '7', 3] it should return 22 because 9 + 3 + 7 + 3 = 22.

---

## Solution 2

```javascript
function sumMix(x) {
  return x.reduce((a, b) => a + Number(b), 0);
}
```

I used `reduce()` and `Number()` to find the solution. `parseInt()` can be used as well.
`Number()` will return a float or (resolved) exponential notation unlike `parseInt()`.

### Tags

`Fundamentals` | `Arithmetic` | `Maths` | `Algorithms` | [Codewars](https://codewars.com)
