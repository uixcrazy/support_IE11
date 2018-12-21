# 🐾 🐾 🐾  support_IE11 🐾 🐾 🐾

## issues

- can't use [Object.values](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_objects/Object/values)

  instead
  ```
  Object.keys(myObject).map(function(key, index) {
    myObject[key] *= 2;
  });
  ```

  ```
  Object.keys(myObject).map((key, index) => (
  ```

- can't use [Array.findIndex](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex) ⤑ instead of ```Array.indexOf```
- others not support ```Array.entries(), Array.find, Array.copyWithin```


- Promise: need to use other library like: [promise-polyfill](promise-polyfill)
⤑ [cnd.jsdelivr](https://cdn.jsdelivr.net/npm/promise-polyfill@8.1.0/dist/polyfill.min.js)

- fetch API: please use [whatwg-fetch](https://www.npmjs.com/package/whatwg-fetch)
⤑ [cnd.jsdelivr](https://cdn.jsdelivr.net/npm/whatwg-fetch@3.0.0/dist/fetch.umd.min.js)
