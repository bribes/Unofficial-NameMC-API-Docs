# NameMC Favorite Server API docs
NameMC has their own system for favoriting servers.

This API's purpose is to get a users favorite servers.

### `GET /v1/namemc/favoriteservers?username=:IGN_Here`
This is the only endpoint for this API.

Parameters are as follows:
- **`IGN_Here`** - the current username of the account

### Possible responses

The API will almost always return HTTP status code `200 OK` and set its `Content-Type` header to `application/json`.

If the user you provide doesn't exist, the API will return HTTP status code `404 Not Found`, and the `Content-Type` header will remain `application/json`.

Here are the different responses that can be returned:

**Returns the users Favorite Servers / HTTP `200`:**
```json
[{"domain":"mc.hypixel.net","icon":"https:\/\/texture.namemc.com\/ad\/bf\/adbf2b8031965b50.png","name":"Hypixel","url":"https:\/\/namemc.com\/server\/mc.hypixel.net"}]
```

**No Favorite Servers / HTTP `200`:**
```json
[]
```

**User Does Not Exist / HTTP `404`:**
```json
{"error":"This user doesn't exist"}
```

**You Didn't Provide The Username Parameter / HTTP `404`:**
```json
{"error":"You didn't supply an account to get a skin hash from! Add the parameter ?username=IGN_HERE."}
```
