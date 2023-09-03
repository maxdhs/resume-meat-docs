# New Phone Who's This API Documentation

```js
const API = "https://new-phone-whos-this-backend.onrender.com";
```

## POST /users/register

### Request:

```js
fetch(`${API}/users/register`, {
  method: "POST",
  headers: { "Content-Type": "application/json" },
  body: JSON.stringify({
    email: "santa@gmail.com",
    password: "pass123@",
  }),
});
```

### Response:

```js
{
  "success": true,
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2MmI2MzBlMS03M2QwLTQyNTEtOTk4Yi05MjcxMjdkZDY3NzQiLCJpYXQiOjE2OTM3NDIyNTJ9.7VR0kSb1amUmcP9iGhqfTIiuM9L5XSZPojkxM1Xg_W8"
}
```

## POST /users/login

### Request:

```js
fetch(`${API}/users/login`, {
  method: "POST",
  headers: { "Content-Type": "application/json" },
  body: JSON.stringify({
    email: "santa@gmail.com",
    password: "pass123@",
  }),
});
```

### Response:

```js
{
  "success": true,
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2MmI2MzBlMS03M2QwLTQyNTEtOTk4Yi05MjcxMjdkZDY3NzQiLCJpYXQiOjE2OTM3NDIyNTJ9.7VR0kSb1amUmcP9iGhqfTIiuM9L5XSZPojkxM1Xg_W8"
}
```

## GET /users/token

### Request:

```js
fetch(`${API}/users/token`, {
  headers: {
    Authorization:
      "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2MmI2MzBlMS03M2QwLTQyNTEtOTk4Yi05MjcxMjdkZDY3NzQiLCJpYXQiOjE2OTM3NDIyNTJ9.7VR0kSb1amUmcP9iGhqfTIiuM9L5XSZPojkxM1Xg_W8",
  },
});
```

### Response:

```js
{
  "success": true,
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOiI2MmI2MzBlMS03M2QwLTQyNTEtOTk4Yi05MjcxMjdkZDY3NzQiLCJpYXQiOjE2OTM3NDIyNTJ9.7VR0kSb1amUmcP9iGhqfTIiuM9L5XSZPojkxM1Xg_W8"
}
```
