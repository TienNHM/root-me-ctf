# Javascript - Obfuscation 2

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FTienNHM%2Froot-me-ctf%2Ftree%2Fmaster%2FWeb-Client%2FJavascript%2520-%2520Obfuscation%25202&count_bg=%2379C83D&title_bg=%232D8FFF&icon=markdown.svg&icon_color=%23092753&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)

## Đề bài

Link: [truy cập ngay 🔗](http://challenge01.root-me.org/web-client/ch12/ch12.html)

![](sc.jpeg)

## Hướng giải

`F12` xem source code:

![](view-src.png)

Ta thấy có đoạn script:

```html
<script type="text/javascript">
	var pass = unescape("unescape%28%22String.fromCharCode%2528104%252C68%252C117%252C102%252C106%252C100%252C107%252C105%252C49%252C53%252C54%2529%22%29");
</script>
```

Ta thử mở tab Console để xem giá trị:

![](decode.png)

Vậy ta thu được pass là `hDufjdki156`.