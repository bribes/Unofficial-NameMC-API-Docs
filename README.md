# www.faav.tk/v1/namemc

Unofficial NameMC API Documentation made by Faav#0130. Documentation for https://namemc.com and www.faav.tk/v1/namemc.

![logo1](https://user-images.githubusercontent.com/52789876/114109154-aa0c7880-98a2-11eb-8925-afa52e0b1404.png)

Need help with using the API? DM me on Discord Faav#0130

### routes
- NameMC Skin Hash API ([documentation](./docs/skinhash.md))
- NameMC Cape Hash API ([documentation](./docs/capehash.md))
- NameMC Capes API ([documentation](./docs/capes.md))
- NameMC Cape Count API ([documentation](./docs/capecount.md))
- NameMC Face Icon API ([documentation](./docs/face.md))
- NameMC Connections API ([documentation](./docs/accounts.md))
- NameMC Connections Count API ([documentation](./docs/accountscount.md))
- NameMC Rank API ([documentation](./docs/rank.md))
- NameMC Emoji API ([documentation](./docs/emoji.md))
- NameMC Custom Font API ([documentation](./docs/font.md))
- NameMC Favorite Servers API ([documentation](./docs/favservers.md))
- NameMC Favorite Servers Count API ([documentation](./docs/favservers_count.md))

### official namemc api
- NameMC Friends API ([documentation](./docs/friends.md))

### usage examples
javascript:

https://www.faav.tk/usage/html
```html
<html>
<head>
	<script>
	var getJSON = function(url, callback) {
	   var xhr = new XMLHttpRequest();
	   xhr.open('GET', url, true);
	   xhr.responseType = 'json';
	   xhr.onload = function() {
	     var status = xhr.status;
	     if (status === 200) {
	       callback(null, xhr.response);
	     } else {
	       callback(status, xhr.response);
	     }
	   };
	   xhr.send();
	};

	getJSON('https://www.faav.tk/v1/namemc/capecount?username=Marc',
	function(err, data) {
	 if (err !== null) {
	   document.getElementById('marc').innerHTML = err;
	 } else {
	   document.getElementById('marc').innerHTML = 'Marc has '+data.formatted+' capes.';
	 }
	});
	</script>
</head>
	<body>
	<p id="marc">Marc has 0 capes.</p>
	</body>
</html>
```
php:

https://www.faav.tk/usage/php
```php 
<?php 
$namemc_api = json_decode(file_get_contents("https://www.faav.tk/v1/namemc/capecount?username=Marc"), false);
$marcs_capes = $namemc_api -> formatted;
 echo '<p>Marc has '.$marcs_capes." capes.</p>";
?>
```

java:

okHttp & Gson:
```java
public static void main(String[] args) {
	final OkHttpClient okHttpClient = new OkHttpClient();
	final Gson gson = new Gson();

	final Request request = new Request.Builder()
		.url("https://www.faav.tk/v1/namemc/capecount?username=Marc")
		.get()
		.build();

	try (final Response response = okHttpClient.newCall(request).execute()) {
		if (response.isSuccessful()) {
			final JsonObject jsonObject = gson.fromJson(response.body().charStream(), JsonObject.class);
			System.out.printf("Marc has %s capes", jsonObject.get("formatted").getAsString());
		}
	} catch (IOException e) {
		e.printStackTrace();
	}
}
```

### warning
NameMC doesn't provide an open API except for their friends API, so this API uses the website itself, so if the website ever changes then the API may be messed up so use at your own risk.

### disclaimer
This API is not affiliated nor indorsed by NameMC, Minecraft, Mojang, or Microsoft.

