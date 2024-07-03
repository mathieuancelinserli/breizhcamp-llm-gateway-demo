# Access validation

```js
const response = await fetch("https://${environment.HOST}/access", {
  headers: {
    Admin: true
  }
});
const data = await response.json();
console.log(data);
```