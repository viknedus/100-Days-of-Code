# 100 days of code, day 5

## Question

> Find the greatest common divisor of two positive integers. The integers can be large, so you need to find a clever solution.
The inputs x and y are always greater or equal to 1, so the greatest common divisor will always be an integer that is also greater or equal to 1
>
> > mygcd(30, 12) will return 6. mygcd(8, 9) returns 1. mygcd(1, 1) returns 1, etc

---

## Solution

```javascript
function mygcd(x,y){
  return y === 0 ? x : mygcd(y, x % y);
}
```

---

## Tags

Algorithms | Optimization | Recursion | [Codewars](https://www.codewars.com/kata/5500d54c2ebe0a8e8a0003fd/)
