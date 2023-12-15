### Change Git Remote URL

In order to change the URL of a Git remote, you have to use the “git remote set-url” command and specify the name of the remote as well as the new remote URL to be changed.

    git remote set-url <remote_name> <remote_url>

For example, let’s say that you want to change the URL of your [Git origin remote](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes).

In order to achieve that, you would use the “set-url” command on the “origin” remote and you would specify the new URL.

    git remote set-url origin https://git-repo/new-repository.git

Congratulations, you successfully changed the URL of your Git remote!

In order to verify that the changes were made, you can use the “git remote” command with the “-v” option (for verbose)

    git remote -v


***
last updated February 6, 2023