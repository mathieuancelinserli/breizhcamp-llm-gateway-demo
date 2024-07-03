# Data Cleanup

TODO: description

```js
const response = await fetch("https://${environment.HOST}/cleanup", {
  method: 'post',
  headers: {
    "content-type": "application/json",
  },
  body: JSON.stringify({
    "credit_card":"4035501000000008"
  })
});

const data = await response.json();
console.log(data);
```

## TODO result