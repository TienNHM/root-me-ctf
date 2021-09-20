# Javascript - Source

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FTienNHM%2Froot-me-ctf%2Ftree%2Fmaster%2FWeb-Client%2FJavascript%2520-%2520Source&count_bg=%2379C83D&title_bg=%232D8FFF&icon=markdown.svg&icon_color=%23092753&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)

## Đề bài

![](sc.jpeg)

Link: [truy cập ngay 🔗](http://challenge01.root-me.org/web-client/ch1/)

![](web.png)
## Hướng giải

`F12` xem source code:

![](view-src.png)

Ta thấy đoạn script sau:

```js
function login(){
    pass=prompt("Entrez le mot de passe / Enter password");
    if ( pass == "123456azerty" ) {
        alert("Mot de passe accepté, vous pouvez valider le challenge avec ce mot de passe.\nYou can validate the challenge using this password.");  }
    else {
        alert("Mauvais mot de passe / wrong password !");
    }
}
```

Vậy password là `123456azerty`.