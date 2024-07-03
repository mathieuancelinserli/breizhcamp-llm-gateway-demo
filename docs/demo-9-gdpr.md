# Data Anonymisation

```ts
const response = await fetch("https://${environment.HOST}/gdpr", {
  method: 'post',
  headers: {
    "content-type": "application/json",
  },
  body: JSON.stringify({
    "name": "Mathieu ANCELIN",
    "age": 38,
    "role": "speaker",
    "languages": ["scala", "java", "javascript", "rust"],
    "email": "mathieu.ancelin@cloud-apim.com"
  })
});

const data = await response.json();
console.log(data);
```