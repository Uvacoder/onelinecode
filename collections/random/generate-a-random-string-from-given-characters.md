---
title: Generate a random string from given characters
category: Random
---

```js
const generateString = (length, chars) =>
    Array(length)
        .fill('')
        .map((v) => chars[Math.floor(Math.random() * chars.length)])
        .join('');

// Example
generateString(10, '0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ');
```
