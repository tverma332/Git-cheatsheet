# Git cheat sheet 

```Note : Text in Bold is Editable```

>git init : Turn Directory into git repository

>git status : To know the current state of your current working directory

>git add **file** : Add file to staging area

> git add  &nbsp;**.**&nbsp;: All the files in current working directory to stage

> git commit -m "**message**" : It will commit all staged files to local repository (-a for automatic staging)

> git log : You can see all the commits/version of your git project. (--oneline for oneline view)

>rm -rf .git : Delete git repository

>touch .gitignore : create .gitignore file, add those file in it that you don't want to be tracked by git.

> git rm --cached **file** : To untrack tracked file

>git restore --staged **file** : To unstage staged file

> git checkout -- **file** : This command takes your file to the last version means it undo all the modifications

> git checkout -f : To restore previous commit

> git config --global alias.**st** **status** : git alias

> git config --global --unset alias.**st** : To remove/unset alias

> git branch : Total branch with name

>git branch -v : Total branch with name and last commit

> git branch **branchname** : To create a new branch

> git checkout **branchname** : Switch to new branch 

>git checkout -b **branchname** : Create and switch at the same time 

> git log --oneline --graph --all : Show all branch with commits

> git branch -d **branchname** : To delete a merged branch

> git merge -D **branchname** : To delete a non-merged branch forcefully

> git merge **branchname** : To merge Branches

> git merge  --abort : To abort the conflict when merging

> git rebase **branchname** : To reabse the branch

> git remote add **remotename** url : Add remote to repo

>git push -u **remotename** **branchname** : push from local repo to remote repo

> git remote -v : To get info about remote

> git clone url : Cloning a github repository

>git remote remove **remotename**: To remove a remote

> git fetch **remotename** **branchname** : To fetch new data for already cloned repo

> git merge **remotename/branchname** : To merge into working directory (Note : Fetch will add only to local repo)

> git pull **remotename** **branchname** : Fetch + Merge

> git show **commitid** : Display the changes in commit

> git stash : To stash file

> git stash list : List of stashed files

> git stash apply **stash@{x}** : Apply stash to staging area(x is any number)

> git stash drop **stash@{x}** : To delete stash after applying

> git clean -f -d : Clean working directory

> git commit --amend : Modify the message of last commit

> git commit --amend --no-edit : Modify the content of last commit

> git checkout **commitid** : Travel to History to any commit

> git switch **-** : Head again on master (undo the Head position) 

>git switch -c **branchname** : Create branch when you made commit in previous snapshot

> git revert **commitid** : Undo the changes of any commit you want

> git revert -n **commitid** : Explicitly commit the revert changes

> git revert --abort : Abort the revert changes

> git reset --soft **commitid** : Delete commits but not file

> git reset --hard **commitid** : Delete commit as well as files