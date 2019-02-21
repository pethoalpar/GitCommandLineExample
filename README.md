# Commands:

## Initialize a local repository

git init - to initialize the local git repository

## Add changes and commit

git add . - add all files to the index

git add [file name] - add a specific file to the index

git add [folder]/ - add a specific folder to the index

git-commit - record changes to the repository

git commit -m "commit message"

git commit --amend -m "New commit message" - change message of last commit

git revert [commit id] - revert a commit

## See the status

git status - show the working tree status

git config --list - see your settings

git diff - see non-staged (non-added) changes to existing files

git diff origin/master - see differences between local changes and master

git diff [first commit id] [second commit id] - see differences between two commits

git diff --name-only [first commit id] [second commit id] - see the files changed between two commits

git show [commit id] -see details of a commit

git log - see recent commit history

git log --all --full-history -- \*/[file name].\* - see a file history

git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit - better log

git fsck - Verifies the connectivity and validity of the objects in the database

## Work with remotes

git remote add origin [url] - add remote repository.

git-push - update remote refs along with associated objects

git push -u origin master

git pull --all - update local branches which track remote branches

git pull [remote] [branch] - update a specific branch

git remote -v - view remote urls

git push origin [branch name] - push the new branch

git remote set-url origin [url] - change the remote url

git clone [repo url] - clone remote repository

## Work with branches

git checkout -b  [branch name] - create and switch to the new branch

git checkout [branch name] - change the branch

git merge [branch name] - merge branch into active branch

git branch -d [branch name] - delete the local branch

git branch - display the branches

git branch -r - display the repositories branches

git push origin --delete [the_remote_branch] - delete repository branch

git fetch [remote] --prune - delete multiple obsolete tracking branches

git diff branch-name - see differences between the current state and a branch

git clean -f - delete all untracked files

## Util

git gc - performs garbage collection on your repository

git reset origin/master - undo non-pushed commits

git reset --hard origin/master - reset to remote state

git for-each-ref --format='%(committerdate) %09 %(authorname) %09 %(refname)' - display the branches and comitter

git show [commit] --stat - show all files modified in this commit

## TAG

git tag [TAG] - create a new tag

git push origin [TAG] - push a tag

## Git config

git config --global user.name "Petho Alpar" - add user name to your config

git config --global user.email "a@a.com" - add email address to your config
