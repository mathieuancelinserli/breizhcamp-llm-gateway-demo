# Prompt Templating

```js
const response = await fetch("https://${environment.HOST}/template", {
  method: 'post',
  headers: {
    "content-type": "application/json",
  },
  body: JSON.stringify({
    "lang": "fr",
    "text": "Hello World !"
  })
});

const data = await response.json();
console.log(data);
```