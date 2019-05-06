### delay

Invokes the provided function after `wait` milliseconds.

Use `setTimeout()` to delay execution of `fn`.
Use the spread (`...`) operator to supply the function with an arbitrary number of arguments.


```js
// 函数、时间、参数
const delay = (fn, wait, ...args) => setTimeout(fn, wait, ...args);
```

```js
delay(
  function(text) {
    console.log(text);
  },
  1000,
  'later'
); // Logs 'later' after one second.
```
