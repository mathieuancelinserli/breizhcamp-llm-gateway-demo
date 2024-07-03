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
        "content": "Can you tell me more about the Cloud APIM company ?"
      }
    ]
  })
});

const data = await response.json();
console.log(data);
```