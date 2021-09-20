# Javascript - Obfuscation 1

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FTienNHM%2Froot-me-ctf%2Ftree%2Fmaster%2FWeb-Client%2FJavascript%2520-%2520Obfuscation%25201&count_bg=%2379C83D&title_bg=%232D8FFF&icon=markdown.svg&icon_color=%23092753&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)

## Đề bài

![](sc.jpeg)

Link: [truy cập ngay 🔗](http://challenge01.root-me.org/web-client/ch4/ch4.html)

![](web.jpeg)

## Hướng giải

`F12` view source:

![](view-src.png)

Ta thấy pass đã được mã hóa như sau:

```js
pass = '%63%70%61%73%62%69%65%6e%64%75%72%70%61%73%73%77%6f%72%64';
```

Decode ta được:

![](decode.png)

Vậy pass là `cpasbiendurpassword`.