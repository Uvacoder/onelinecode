---
title: Get the last date in the month of a date
category: Date Time
---

```js
const getLastDate = (d = new Date()) => new Date(d.getFullYear(), d.getMonth() + 1, 0);
```
