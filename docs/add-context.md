# Add context to your API

```js

const response = await fetch("https://${environment.HOST}/context", {
  method: 'post',
  headers: {
    "content-type": "application/json",
  },
  body: JSON.stringify({
    "messages": [
      {
        "role": "user",
        "content": "peux tu m'en dire plus sur la societe cloud apim ?"
      }
    ]
  })
});

const data = await response.json();
console.log(data);
```