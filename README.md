<p align=center>
<img src="https://docs.faav.tk/logo.svg">
</p>

<p align=center>
Unofficial NameMC API Documentation made by Faav.<br>
Documentation for https://namemc.com and www.faav.tk/v1/namemc.<br><br>
</p>

---
<br>

## Contents
- [About](#about)

- [Limitations](#limitations)

- [Routes](#routes)

- [Official NameMC API](<#official-namemc-api>)

- [Usage Examples](<#usage-examples>)
	- [JavaScript](#javascript)
	- [PHP](#php)
	- [Java](#java)
<br>

## About
I created this API for people who need to use NameMC's database in a automated way.

<br>

## Limitations
This API scrapes the NameMC website in order to provide accurate responses. If the NameMC layout changes or goes offline, this API will provide inaccurate information or will not function at all. Please keep this in mind while using this API. 

<br>

## Routes
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

<br>

## Official NameMC API
- NameMC Friends API ([documentation](./docs/friends.md))

<br>

## Usage Examples

### JavaScript:

[See it in action](https://www.faav.tk/usage/html)
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
<br>

### PHP:

[See it in action](https://www.faav.tk/usage/php)
```php 
<?php 
$namemc_api = json_decode(file_get_contents("https://www.faav.tk/v1/namemc/capecount?username=Marc"), false);
$marcs_capes = $namemc_api -> formatted;
 echo '<p>Marc has '.$marcs_capes." capes.</p>";
?>
```
<br>

### Java:

#### OkHttp & Gson:
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
<br>

## Contributions
Thank you JerreBor (Jero) for the Java usage example and the better Read Me file, and thank you lucky swede for the documentation template.

<br>

## Disclaimer
This API is not affiliated nor indorsed by NameMC, Minecraft, Mojang, and/or Microsoft.

