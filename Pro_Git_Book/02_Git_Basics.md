# Git Basics

The command to initialize a git repository in the current directory:
```bash
git init
```
The command to clone a repository at https://github.com/libgit2/libgit2:
```bash
git clone https://github.com/libgit2/libgit2
```
If you want to clone the above repository, but you you want it to be placed in a new directory to be called fuzzyturtles instead:
```bash
git clone https://github.com/libgit2/libgit2 fuzzyturtles
```
A command to determine the state of the files in a git repo:
```bash
git status
```
Tell git to begin tracking a file called myfile.txt in your repo:
```bash
git add myfile.txt
```
A command to see what you've changed within the repo but not yet staged:
```bash
git diff
```
A command to see what you've staged so far in a repo:
```bash 
git diff --cached
```
A command to list the commits made in a repo in reverse chronological order:
```bash
git log
```
A command to list the commits like above, but formatting each commit on a single line:
```bash
git log --pretty=oneline
```
A command to list the last 42 commits:
```bash
git log -42
```
A command to redo the last commit after making forgotten changes and staging them:
```bash
git commit --amend
```
A command to unstage file myfile.txt:
```bash
git reset HEAD myfile.txt
```
Revert myfile.txt to what it looked like when you last committed or cloned it:
```bash
git checkout -- myfile.txt
```
List the shortnames of each remote handle you've specified:
```bash
git remote
```
A version of the above command that shows you the URLs git has stored for the shortname, for use when reading/writing to that remote:
```bash
git remote -v
```
Add a new remote git repo at [url] called [shortname]:
```bash
git remote add [shortname] [url]
```
Given remote repo called [shortname], get all info in that repo that you don't have yet in your local repo:
```bash
git fetch [shortname]
```
Push changes to [remote] [branch]:
```bash
git push [remote] [branch]
```
See more info about a particular remote:
```bash
git remote show [remote]
```
Rename shortname of remote thing1 to thing2:
```bash
git remote rename thing1 thing2
```
Remove remote [shortname]:
```bash
git remote remove [shortname]
```
List your tags:
```bash
git tag
```
Search for tags that match pattern v1.8.5*:
```bash
git tag -l "v1.8.5*"
```
Create an annoted tag called v1.1 with message "I'm a l33t hax0r":
```bash
git tag -a v1.1 -m "I'm a l33t hax04"
```
See tag data about tag v1.1:
```bash
git show v1.1
```
Create a lightweight tag called v1.1.1:
```bash
git tag v1.1.1
```
Tag the commit that starts with checksum 9fceb02 with v1.3:
```bash
git tag -a v1.3 9fceb02
```
Push tag v1.4 to remote orgin:
```bash
git push origin v1.4
```
Push all tags that are not already there to remote origin:
```bash
git push origin --tags
```
Delete tag v1.5 from your local repo:
```bash
git tag -d v1.5
```
Delete tag v1.6 from remote origin:
```bash
git push origin --delete v1.6
```

