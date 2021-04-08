# NameMC Custom Font API docs
NameMC has their own system for having Custom Fonts.

This API's purpose is to get a users Custom Font.

### `GET /v1/namemc/font?username=:IGN_Here`
This is the only endpoint for this API.

Parameters are as follows:
- **`IGN_Here`** - the current username of the account
### Possible fonts
- Amarante
- Carter One
- Coda
- Concert One
- Emilys Candy
- Griffy
- Henny Penny
- Kalam
- Kelly Slab
- Lacquer
- Lobster
- Merienda
- Mystery Quest
- PT Mono
- Pacifico
- Righteous
- Rye
- Sancreek
- Sofia
- Special Elite
- Spicy Rice
- Spirax
- Stardos Stencil
- Underdog
- UnifrakturMaguntia

### Possible responses

The API will almost always return HTTP status code `200 OK` and set its `Content-Type` header to `application/json`.

If the user you provide doesn't exist, the API will return HTTP status code `404 Not Found`, and the `Content-Type` header will remain `application/json`.

Here are the different responses that can be returned:

**Returns the Font / HTTP `200`:**
```json
{"font":"Spirax"}
```

**No Font / HTTP `200`:**
```json
{"font":null}
```

**User Does Not Exist / HTTP `404`:**
```json
{"error":"This user doesn't exist"}
```

**You Didn't Provide The Username Parameter / HTTP `404`:**
```json
{"error":"You didn't supply an account to get a skin hash from! Add the parameter ?username=IGN_HERE."}
```
