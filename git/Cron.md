I had to add the document root to the php include path to get the cron working.

Here's a good article on doing that:
 [Setting the PHP include path](https://www.a2hosting.com/kb/developer-corner/php/php-include-paths)

Here's a good article on cron jobs for beginners [A Beginners Guide To Cron Jobs](https://ostechnix.com/a-beginners-guide-to-cron-jobs/)

Our hosting provider uses [cpanel](https://cpanel.net/) and has a graphical user interface for cron jobs.

Our cron job runs every 15 minutes and looks something like this:

`*/15  *  *  *  * /usr/local/bin/php /home/username/your path to >/Zotlabs/Daemon/Master.php`

Next let's look at [Installing addons](https://github.com/socialatm/test/wiki/Installing-addons)

