Hubzilla provides a platform for powerful extensions called addons. These are independent modules that can be downloaded and activated by the hub admin to provide additional capabilities or custom features. Hubzilla provides a a wealth of hooks through the core functions, allowing addons to extend functionality.

Collections of plugins are added as repositories: typically git repos for convenient downloading and updating. All officially supported plugins are in the [hubzilla-addons](https://github.com/socialatm/addons.git) repo.

***

* Log into you website and open the [command line teminal](https://www.freecodecamp.org/news/command-line-for-beginners)
* We log in remotely using [SSH](https://www.ssh.com/academy/ssh/protocol)
* For additional assistance check with your hosting provider.
* Make sure you are in your website directory  `cd /path/to/website/folder`
* Clone the addon repository. We'll give this repository a nickname of 'socialatm'.
*     util/add_addon_repo https://github.com/socialatm/addons.git socialatm
*  You can pull in other hubzilla addon repositories by giving them different nicknames.
* To update your addons at any time issue the update command:
*     util/update_addon_repo socialatm

***

Go to `https://yourwebsite/admin/addons/` to view your newly installed addons.  
Click on the checkmark box next to any addons you wish to enable.

***

### More command line options

		util/addons list             # list installed addons
		util/addons list all         # list all addons (*)= installed, (!)= disabled due to version compatibility
		util/addons install foo      # install addon named 'foo'
		util/addons uninstall foo    # uninstall addon named 'foo'
		util/addons reinstall        # reinstall all plugins



