---
title: Check if a given integer is a prime number
category: Validator
---

```js
const isPrime = (num) =>
    num > 1 &&
    Array(Math.floor(Math.sqrt(num)) - 1)
        .fill(0)
        .map((_, i) => i + 2)
        .every((i) => num % i !== 0);
```
