# 100 days of code, day 4

## Question

> Given the head of a singly linked list, reverse the list, and return the reversed list.
>
> > Input: head = [1, 2, 3, 4, 5]. Output: [5, 4, 3, 2, 1]

---

## Solution

```javascript
var reverseList = function (head) {
  let [prev, cur] = [null, head];
  while (cur) {
    [cur.next, prev, cur] = [prev, cur, cur.next];
  }
  return prev;
};
```

---

## Tags

`Algorithms` | `Arrays` | [Leetcode](https://leetcode.com/problems/reverse-linked-list/)
