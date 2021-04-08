# NameMC Favorite Servers Count API docs
NameMC has their own system for favoriting servers.

This API's purpose is to get the number of servers the user has favorited.

### `GET /v1/namemc/emoji?username=:IGN_Here`
This is the only endpoint for this API.

Parameters are as follows:
- **`IGN_Here`** - the current username of the account

### Possible responses

The API will almost always return HTTP status code `200 OK` and set its `Content-Type` header to `application/json`.

If the user you provide doesn't exist, the API will return HTTP status code `404 Not Found`, and the `Content-Type` header will remain `application/json`.

Here are the different responses that can be returned:

**Returns Amount of Servers Favorited / HTTP `200`:**
```json
{"formatted":"2","value":2}
```

**No Favorite Servers / HTTP `200`:**
```json
{"formatted":"0","value":0}
```

**User Does Not Exist / HTTP `404`:**
```json
{"error":"This user doesn't exist"}
```

**You Didn't Provide The Username Parameter / HTTP `404`:**
```json
{"error":"You didn't supply an account to get a skin hash from! Add the parameter ?username=IGN_HERE."}
```
