# NameMC Friends API docs
NameMC has their own API for friends.

### `GET https://api.namemc.com/profile/UUID_Here/friends`
This is the only endpoint for this API.

Parameters are as follows:
- **`UUID_Here`** - the UUID of the account

### Possible responses

The API will almost always return HTTP status code `200 OK` and set its `Content-Type` header to `application/json`.

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
