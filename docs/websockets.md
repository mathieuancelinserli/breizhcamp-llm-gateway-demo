# WebSockets : handle hate speech

```ts
const response = await fetch(https://${environment.HOST}/websockets, 
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