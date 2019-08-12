# Git Branches

Create a new branch called feature2 (i.e. a new pointer to the same commit you're currently on):
```bash
git branch feature2
```
Switch the new branch you created called feature2, in effect moving the HEAD to point to the new branch:
```bash
git checkout feature2
```
A command that does the above two commands at the same time:
```bash
git checkout -b feature2
```
If you are on branch feature2, the commands to merge feature2 branch into master branch:
```bash
git checkout master
git merge feature2
```
Delete an already merged branch called hotfix:
```bash
git branch -d hotfix
```
If you run into a merge conflict, a command to see which files are unmerged:
```bash
git status
```
The command to use a graphical tool to resolve merge conflicts:
```bash
git mergetool
```
After all conflicts in a merge are fixed, how do you conclude the merge:
```bash
git commit
```
Display a listing of current branches in repo:
```bash
git branch
```
Display a listing of current branches with last commit for each:
```bash
git branch -v
```
Display a branch list with the branch you're on and any other branches you have already merged into it:
```bash
git branch --merged
```
The same as the above command, but with other branches that have not been merged yet into current branch:
```bash
git branch --no-merged
```
Create a new branch called imstoopid that starts where remote branch origin/imsmart is:
```bash
git fetch origin
git checkout -b imstoopid origin/imsmart
```
List the tracking branches you have set up:
```bash
git branch --v
```
