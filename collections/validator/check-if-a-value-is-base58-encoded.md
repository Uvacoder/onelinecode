---
title: Check if a value is base58 encoded
category: Validator
---

```js
// It doesn't accept the I, O, l characters
const isBase58 = (value) => /^[A-HJ-NP-Za-km-z1-9]*$/.test(value);
```
