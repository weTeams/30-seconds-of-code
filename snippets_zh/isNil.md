### isNil

检测输入值是否为 null 或 undefined
Returns `true` if the specified value is `null` or `undefined`, `false` otherwise.

Use the strict equality operator to check if the value and of `val` are equal to `null` or `undefined`.

```js
const isNil = val => val === undefined || val === null;
```

```js
isNil(null); // true
isNil(undefined); // true
```
