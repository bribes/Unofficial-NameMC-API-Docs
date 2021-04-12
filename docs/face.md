# NameMC Face Icon API docs
NameMC has their own Face Images.

This API's purpose is to get the Face Icon of a player.

### `GET /v1/namemc/face?username=:IGN_Here`
This is the only endpoint for this API.

Parameters are as follows:
- **`IGN_Here`** - the current username of the account

### Possible responses

The API will almost always return HTTP status code `200 OK` and set its `Content-Type` header to `application/json`.

If the user you provide doesn't exist, the API will return HTTP status code `404 Not Found`, and the `Content-Type` header will remain `application/json`.

Here are the different responses that can be returned:

**Returns the Images / HTTP `200`:**
```json
{"icon_url":"https:\/\/render.namemc.com\/skin\/2d\/face.png?skin=a7c87dca2251c5b6&overlay&scale=2","skin_url":"https:\/\/texture.namemc.com\/a7\/c8\/a7c87dca2251c5b6.png"}
```

**User Does Not Exist / HTTP `404`:**
```json
{"error":"This user doesn't exist"}
```

**You Didn't Provide The Username Parameter / HTTP `404`:**
```json
{"error":"You didn't supply an account to get a face from! Add the parameter ?username=IGN_HERE."}
```

