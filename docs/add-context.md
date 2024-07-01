# Add context to your API

```ts
const response = await fetch(https://${environment.HOST}/context, 
{
  headers: {
    "content-type": "application/json",
  },
  body: {
    "message": "Connais-tu le BreizhCamp ???"
  }
});

const data = await response.json();
console.log(data);
```