# 100 days of code, day 3

## Question
> You will be given an array of numbers in which two numbers occur once and the rest occur only twice. Your task will be to return the sum of the numbers that occur only ONCE.
> > For example, repeats([4,5,7,5,4,8]) = 15 because only the numbers 7 and 8 occur once, and their sum is 15. Every other number occurs twice.

---

## Solution

```javascript
function repeats(arr){
  var z = arr.filter(function(a) {
    return arr.filter(function(b) {
      return b == a;
      }).length == 1;
    });  return z.reduce((x, y) => x + y, 0);
};
```
I used `filter()` and `reduce()` to achieve this.

---

## Tags

Algorithms | Arrays | Sorting | [Codewars](https://codewars.com)