---
title: Check if a value is a function
category: Function
---

```js
const isFunction = (v) =>
    ['[object Function]', '[object GeneratorFunction]', '[object AsyncFunction]', '[object Promise]'].includes(
        Object.prototype.toString.call(v)
    );

// Examples
isFunction(function () {}); // true
isFunction(function* () {}); // true
isFunction(async function () {}); // true
```
