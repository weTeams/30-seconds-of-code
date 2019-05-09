### inRange

Checks if the given number falls within the given range.

检查所给的数字是否在范围之内

Use arithmetic comparison to check if the given number is in the specified range.
If the second parameter, `end`, is not specified, the range is considered to be from `0` to `start`.

<!--  如果 结尾或者开始比结尾大 交换-->

```js
const inRange = (n, start, end = null) => {
        console.log(end && start,end && start > end)
  if (end && start > end) [end, start] = [start, end];
  return end == null ? n >= 0 && n < start : n >= start && n < end;
};
```

```js
inRange(3, 2, 5); // true
inRange(3, 5, 2); // true
inRange(3, 4); // true
inRange(2, 3, 5); // false
inRange(3, 2); // false
```
