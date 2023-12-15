At some point will will separate the frontend client from the backend server.  
This seems like a good time to start a list of what goes where.

### Client
* view folder

### Server
* Zotlabs folder
* include folder
* index.php file

In our Zotlabs/Modules folder find this line:

    $o = replace_macros(get_markup_template('notifications_widget.tpl'), [
			'$notifications' => $notifications,
			'$no_notifications' => t('No new notifications'),
			'$loading' => t('Loading'),
		]);
		return $o;

and of course the name of the template will be different depending on which module you are in.

the **replace_macros** line is basically the divider between the server and the client. The lines below it
are the variables that get passed to the template.

wondering what those variables are? Add this below:

    $arr = [
			'$notifications' => $notifications,
			'$no_notifications' => t('No new notifications'),
			'$loading' => t('Loading'),
		]);

	print("<pre>".print_r($arr,true)."</pre>");
        exit;

That will print a readable list of the variables and their values, **key=>value**

In theory at least from here we could [json_encode](https://www.php.net/manual/en/function.json-encode.php) the variables
and [echo](https://www.php.net/manual/en/function.echo) them to a javascript/node type frontend.  
Something to think about.

