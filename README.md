# CheckSSL

:lock:Check your site's SSL status

[![Author](https://img.shields.io/badge/Author-Sukka-b68469.svg?style=flat-square)](https://skk.moe)
![Travis](https://img.shields.io/travis/SukkaLab/ssl.svg?style=flat-square)
[![License](https://img.shields.io/github/license/sukkaw/CheckSSL.svg?style=flat-square)](./LICENSE)

## Demo

https://lab.skk.moe/ssl

## Usage

First clone this repo:

```bash
$ git clone https://github.com/SukkaW/CheckSSL.git
$ cd CheckSSL
```

Then give script permission to execute:

```bash
$ chmod +x checker.sh
```

Run `checker.sh` with your domain, just like

```bash
# Example
$ ./checker.sh skk.moe www.skk.moe blog.skk.moe lab.skk.moe
```

You will get a `ct.json` file at `output` directories with format like:

```json
[{
	"domain": "skk.moe",
	"subject": "C=US; ST=CA; L=San Francisco; O=CloudFlare, Inc.; CN=sni.cloudflaressl.com",
	"start": "2018-09-14 00:00:00 GMT",
	"expire": "2019-09-14 12:00:00 GMT",
	"issuer": "C=US; ST=CA; L=San Francisco; O=CloudFlare, Inc.; CN=CloudFlare Inc ECC CA-2",
	"status": "Valid",
	"statuscolor": "success",
	"check": "2018-10-20 15:23:54",
	"remain": "328"
}, {
	"domain": "www.skk.moe",
	"subject": "C=US; ST=CA; L=San Francisco; O=CloudFlare, Inc.; CN=sni.cloudflaressl.com",
	"start": "2018-09-17 00:00:00 GMT",
	"expire": "2019-09-17 12:00:00 GMT",
	"issuer": "C=US; ST=CA; L=San Francisco; O=CloudFlare, Inc.; CN=CloudFlare Inc ECC CA-2",
	"status": "Valid",
	"statuscolor": "success",
	"check": "2018-10-20 15:23:54",
	"remain": "331"
}]
```

## Author

**CheckSSL** © [Sukka](https://github.com/SukkaW), Released under the [MIT](./LICENSE) License.

> [Personal Website](https://skk.moe) · [Blog](https://blog.skk.moe) · GitHub [@SukkaW](https://github.com/SukkaW) · Telegram Channel [@SukkaChannel](https://t.me/SukkaChannel)

