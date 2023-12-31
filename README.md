# twitter-web-auth
Generates Twitter web auth token

### Get auth token

```typescript
const response = await getAuthToken({ email, username, password });
// response
//  {
//    "authToken": "<authToken>",
//    "bearer": "<bearer>",
//    "csrfToken": "<csrfToken>",
//    "guestToken": "<guestToken>"
//  }
```

### Get only guest token

```typescript
const response = await getAuthToken();
// response
//  {
//    "bearer": "<bearer>",
//    "csrfToken": "<csrfToken>",
//    "guestToken": "<guestToken>"
//  }
```

### Generate new CSRF Token
```typescript
const newCsrfToken = generateCsrfToken();
```