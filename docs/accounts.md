# NameMC Connections API docs
NameMC has their own system for linking your other connections like Discord, Github, and etc.

This API's purpose is to get the connections a user has.

### `GET /v1/namemc/accounts?username=:IGN_Here`
This is the only endpoint for this API.

Parameters are as follows:
- **`IGN_Here`** - the current username of the account

### Possible responses

The API will almost always return HTTP status code `200 OK` and set its `Content-Type` header to `application/json`.

If the user you provide doesn't exist, the API will return HTTP status code `404 Not Found`, and the `Content-Type` header will remain `application/json`.

Here are the different responses that can be returned:

**Returns the Users Connections / HTTP `200`:**
```json
[{"content":"Faav#0130","icon":"https:\/\/static.namemc.com\/i\/service\/discord.svg","title":"Discord"},{"icon":"https:\/\/static.namemc.com\/i\/service\/github.svg","title":"GitHub","url":"https:\/\/github.com\/FaavXD"},{"icon":"https:\/\/static.namemc.com\/i\/service\/reddit.svg","title":"Reddit","url":"https:\/\/www.reddit.com\/user\/FaavXD"},{"icon":"https:\/\/static.namemc.com\/i\/service\/steam.svg","title":"Steam","url":"https:\/\/steamcommunity.com\/id\/f4av"},{"icon":"https:\/\/static.namemc.com\/i\/service\/twitter.svg","title":"Twitter","url":"https:\/\/twitter.com\/FaavXD"},{"icon":"https:\/\/static.namemc.com\/i\/service\/youtube.svg","title":"YouTube","url":"https:\/\/www.youtube.com\/channel\/UCzG5jazKOD2n0jCSdraTzGA"}]
```

**No Connections / HTTP `200`:**
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
