# Data Cleanup

Here we use the LLM to hide sensitive informations to avoid data leaks. In this particular case, the LLM hides a credit card number and add contextual informations about the card.

## Call the API

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

## Result

```js
{
  "credit_card": "************0008 (Visa)"
}
```