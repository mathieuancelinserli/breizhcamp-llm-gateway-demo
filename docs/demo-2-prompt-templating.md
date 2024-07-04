# Prompt Templating

TODO: description

## Call the API

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

## Result

```js
{
  "generations": [
    {
      "message": {
        "role": "assistant",
        "content": "Bonjour le monde !"
      }
    }
  ],
  "metadata": {
    "rate_limit": {
      "requests_limit": 10000,
      "requests_remaining": 9999,
      "tokens_limit": 60000,
      "tokens_remaining": 59963
    },
    "usage": {
      "prompt_tokens": 23,
      "generation_tokens": 4
    }
  }
}
```