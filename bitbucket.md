## BitBucket guide

__Create new branch:__

 1. Go to folder of your repository.
 2. `git branch <name>` - point to new branch.
 3. `git checkout <name_of_branch>` - start using new branch.
 4. `git status` - check if you are working on requested branch.
 5. `git add` - add changes.
 6. `git commit -m "update"`

__Now if you want to merge and make new master:__

 `git status`
 `git checkout master`
 `git merge <name_of_branch>`
 `git branch -d <name_of_branch>` - delete branch since its master now and we dont use it anymore.

__Usefull commands:__

 `git clone -b <branch_name> <remote_repository_URL>` - clone specific branch.
