# Data enrichment

```js
const response = await fetch("https://${environment.HOST}/enrich", {
  method: 'post',
  headers: {
    "content-type": "application/json",
  },
  body: JSON.stringify({
    "email": "mathieu.ancelin@cloud-apim.com",
    "city": "Poitiers"
  })
});
const data = await response.json();
console.log(data);
```