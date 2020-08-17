## BitBucket guide

1. Go to folder of your repository.
2. `git branch <name>` - point to new branch.
3. `git checkout <name_of_branch>` - start using new branch.
4. `git status` - check if you are working on requested branch.
5. `git add` - add changes.
6. `git commit -m "update"`

	__Now if you want to merge and make new master:__
	1. `git status`
	2. `git checkout master`
	3. `git merge <name_of_branch>`
	4. `git branch -d <name_of_branch>` - delete branch since its master now and we dont use it anymore.
