---
title: Get the base URL without any parameters
category: String
---

```js
const baseUrl = (url) => (url.indexOf('?') === -1 ? url : url.slice(0, url.indexOf('?')));

// Or
// Note that `includes` isn't supported in IE 11
const baseUrl = (url) => (url.includes('?') ? url.slice(0, url.indexOf('?')) : url);

// Or
const baseUrl = (url) => url.split('?')[0];

// Example
baseUrl('https://domain.com/path/sub/path?foo=bar&hello=world'); // 'https://domain.com/path/sub/path'
```
