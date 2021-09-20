# Javascript - Authentication 2

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FTienNHM%2Froot-me-ctf%2Ftree%2Fmaster%2FWeb-Client%2FJavascript%2520-%2520Authentication%25202&count_bg=%2379C83D&title_bg=%232D8FFF&icon=markdown.svg&icon_color=%23092753&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)

## Đề bài

Link: [truy cập ngay 🔗](http://challenge01.root-me.org/web-client/ch11/)

![](sc.jpeg)

## Hướng giải

Xem sourc code ta thấy có sử dụng 1 hàm `connexion();`

![](view-src.png)

Mở file `login.js`:

![](view-js.png)

```javascript
function connexion(){
    var username = prompt("Username :", "");
    var password = prompt("Password :", "");
    var TheLists = ["GOD:HIDDEN"];
    for (i = 0; i < TheLists.length; i++)
    {
        if (TheLists[i].indexOf(username) == 0)
        {
            var TheSplit = TheLists[i].split(":");
            var TheUsername = TheSplit[0];
            var ThePassword = TheSplit[1];
            if (username == TheUsername && password == ThePassword)
            {
                alert("Vous pouvez utiliser ce mot de passe pour valider ce challenge (en majuscules) / You can use this password to validate this challenge (uppercase)");
            }
        }
        else
        {
            alert("Nope, you're a naughty hacker.")
        }
    }
}
```

Ta thấy `username` và `password` lần lượt là 2 phần tử của mảng `TheSplit`:

```javascript
TheUsername = "GOD";
ThePassword = "HIDDEN";
```

Dùng password trên để submit 🌟.