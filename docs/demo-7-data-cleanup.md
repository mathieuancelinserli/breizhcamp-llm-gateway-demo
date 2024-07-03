# Data Cleanup

```ts
const response = await fetch(https://${environment.HOST}/cleanup, 
{
  headers: {
    "content-type": "application/json",
  },
  body: {
    "message": "test"
  }
});

const data = await response.json();
console.log(data);
```