# Data enrichment

```ts
const response = await fetch(https://${environment.HOST}/enrich, 
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