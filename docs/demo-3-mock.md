# Mock Responses

TODO: description

## Call the API

```js
const response = await fetch("https://${environment.HOST}/mock");
const data = await response.json();
console.log(data);
```

## Result

```js
[
  {
    "email": "user1@example.com",
    "name": "Alice",
    "age": 25,
    "address": "123 Main St"
  },
  {
    "email": "user2@example.com",
    "name": "Bob",
    "age": 30,
    "address": "456 Elm St"
  },
  {
    "email": "user3@example.com",
    "name": "Charlie",
    "age": 35,
    "address": "789 Oak St"
  },
  {
    "email": "user4@example.com",
    "name": "Diana",
    "age": 40,
    "address": "234 Maple St"
  },
  {
    "email": "user5@example.com",
    "name": "Eve",
    "age": 45,
    "address": "567 Pine St"
  }
]
```