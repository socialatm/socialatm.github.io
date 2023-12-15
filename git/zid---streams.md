Adding the 'zid' parameter to any request URL is why you don't need to be known on the target server. If it doesn't know you, it will discover you AND authenticate/authorise your session.

The usefulness of something like this is demonstrated by the utl/nsh app in streams. This combines OpenWebAuth with WebDAV and is a command line tool that sees cloud storage in the fediverse as one gigantic file system.  

$ util/nsh
logging in...
Hi -  mike

macgirvin.com:/mike/> ls
2022/
2023/
Profile%20Photos/ ("Profile Photos")
20221208_190817.jpg

macgirvin.com:/mike/> connect mario@hub.somaton.com 

hub.somaton.com:/mario/> ls
2021-01/
2021-02/
2021-03/
2021-04/
2021-05/
2021-06/
2021-07/
2021-08/
2021-10/
2021-11/
2021-12/
2022-01/
2022-02/
2022-03/
2022-04/
2022-06/
2022-07/
2022-08/
2022-09/
2022-10/
2022-11/
2022-12/
2023-01/
Cover%20Photos/ ("Cover Photos")
Profile%20Photos/ ("Profile Photos")
rts_mdt_demo/
testter1/

hub.somaton.com:/mario/> connect scott@scottstolz.com 

scottstolz.com:/scott/> ls
2022-11/
images/
memes/
screenshots/
newhub-menu-test-1.png

scottstolz.com:/scott/> get newhub-menu-test-1.png

scottstolz.com:/scott/> quit

[macgirvin@stayton] ~/macgirvin (dev)
$ ls newhub-menu-test-1.png 
newhub-menu-test-1.png
[macgirvin@stayton] ~/macgirvin (dev)
$

The brilliant part of all this is that just like the web interface - you only see files you're allowed to see.

Most of the time we're only using OpenWebAuth for authorisation (access control), but for some interfaces we also use it for authentication. For instance if you click on the channel page to 'moderate' a channel on another site where you have moderation permissions, it will log you in to that channel with reduced permissions. It's also used for API authentication so you can clone your photos without requiring login.
