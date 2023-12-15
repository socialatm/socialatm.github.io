Here are the steps we took to install it.

* Get a domain name.
* Get web hosting. We're on shared hosting running a [Lightspeed server](https://www.litespeedtech.com/products/litespeed-web-server)
* Get a SSL certificate. Our hosting provider had it all set up but if yours does not a good free option is [Lets Encrypt](https://letsencrypt.org/).
* No, you can not use a self signed certificate, go without one, or host it on localhost.
* Upload your files to your [document root](https://www.pcmag.com/encyclopedia/term/document-root)
* You can use a [subdomain](https://www.pcmag.com/encyclopedia/term/subdomain) if you wish but you can not use a [subdirectory](https://www.pcmag.com/encyclopedia/term/subdirectory)
* We set up a blank git repository and did a `git clone` to install our files but this step is optional and you can just upload the files if you wish.
* Set up a blank database and add a database user. Do not add any tables to the database. Save your database name, user and password in a secure spot because you will need that info during the web install. You can use either [MySql](https://www.mysql.com/) or [postgresql](https://www.postgresql.org/). MySql was the original hubzilla database and we were already familiar with it so we went with that.
* Open **https://yourdomain.com** in your web browser and the web installer will start. Of course you'll replace yourdomain.com with your actual domain name.
* The web installer will give you the chance to fix any php issues, add your database information and add the administrator email address and your timezone. Unless you're using a custom or remote database leave the ****Database Server Name**** and ****Database Port**** as is
* Be sure to take note of the exact administrator email address because you're going to need it to register as Admin.
* Now you can register as admin. You're required to use the exact administrator email address that you used during the install process and you must be the first person to register.
* You can click the register link at the bottom of the install success page or from the https://yourdomain.com home page.
* Your install is now complete and you're ready to use your website.
* If you have any issues along the way you can post them [here](https://github.com/socialatm/core/issues) and we'll do our best to help.
* Next we will [get cron jobs working](https://github.com/socialatm/test/wiki/Cron)


