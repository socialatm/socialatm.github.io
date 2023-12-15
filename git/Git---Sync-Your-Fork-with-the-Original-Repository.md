
    # Add a new remote upstream repository
    git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git

    # Sync your fork
    git fetch upstream
    git checkout main # or whatever branch you want to sync
    git merge upstream/main

Verify your changes with:

    git remote -v

### To remove an upstream:

    git remote remove upstream

Verify your changes with:

    git remote -v