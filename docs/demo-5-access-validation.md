# Access validation

TODO: description

## Call the API

```js
const response = await fetch("https://${environment.HOST}/access", {
  headers: {
    Admin: true
  }
});
const data = await response.json();
console.log(data);
```

## Result

```js
{
  "method": "GET",
  "path": "/access",
  "headers": {
    "host": "mirror.otoroshi.io",
    "accept": "*/*",
    "sozu-id": "01J1YK6WZCEHYENYKR9FFYB3BP, 01J1YK5DW3R3BEJ2R1E1EZ4P4G",
    "forwarded": "proto=https;for=0.0.0.0:60006;by=0.0.0.0, proto=https;for=0.0.0.0:49902;by=0.0.0.0",
    "user-agent": "curl/8.1.2",
    "x-forwarded-port": "443",
    "x-forwarded-for": "0.0.0.0",
    "x-forwarded-proto": "https"
  },
  "body": ""
}
```