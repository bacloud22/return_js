# return_js
Quick return from a called function

```js
function return42 () {
  return 42
}
```

```js
// Calling function
function main() {
  if (return42() === 42) return return42()
  else {
    // continue
  }
}
```

There should be a way for `main()` to decide to return or to continue without an if-else

Like the following

```js
function main() {
  __return__ return42()
  //... rest of code when return42() returns a value other than 42 !!!
}
```

Agree ?
