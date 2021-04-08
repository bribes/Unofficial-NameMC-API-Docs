# NameMC Friends API docs
NameMC has their own system for caching capes.

This API's purpose is to get all capes a user owns according to NameMC.

### `GET https://api.namemc.com/profile/UUID_Here/friends`
This is the only endpoint for this API.

Parameters are as follows:
- **`UUID_Here`** - the UUID of the account

### Possible responses

The API will almost always return HTTP status code `200 OK` and set its `Content-Type` header to `application/json`.

If the user you provide doesn't exist, the API will return HTTP status code `404 Not Found`, and the `Content-Type` header will remain `application/json`.

Here are the different responses that can be returned:

**Returns the Users Friends / HTTP `200`:**
```json
[
  {
    "uuid": "403e6cb7-a6ca-440a-8041-7fb1e579b5a5",
    "name": "CoderTim"
  },
  {
    "uuid": "07e7e8a9-7ee8-4c74-8ee7-77f13e5ed55f",
    "name": "Core"
  },
{
    "uuid": "b50c8925-2346-451f-91e0-ce7c0b1b7256",
    "name": "Fungi"
  },
  {
    "uuid": "fae14fed-b1b9-4938-8b6c-250e7db818a1",
    "name": "MeeZoid"
  },
  {
    "uuid": "91d8cbb7-4753-471f-af93-75bae55ac8ce",
    "name": "NotNico"
  }
]
```

**No Friends / HTTP `200`:**
```json
[]
```

**Invalid UUID / HTTP `400`:**
```
Bad Request
```

**You Didn't Provide The Username Parameter / HTTP `404`:**
```json
{"error":"You didn't supply an account to get a skin hash from! Add the parameter ?username=IGN_HERE."}
```
