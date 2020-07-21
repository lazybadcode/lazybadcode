---
title: git-command-line
date: 2020-07-09 23:00:28
tags:
---

### Git Command

![Image of Branch](/images/git-branches-merge.png)

#Set user global
``` bash
$ git config --global user.name "FIRST_NAME LAST_NAME"

$ git config --global user.email "MY_NAME@example.com"
```

#Get config
``` bash
$ git config -l --show-origin

$ git config --global -l --show-origin
```

#Clone
``` bash
$ git clone origin
```

#Status
``` bash
$ git status
```

#Diff
``` bash
$ git diff [filename]
```

#Add
``` bash
$ git add .

#keep and modified 
$ git reset HEAD [filename]

#unkeep and modified
$ git reset HEAD --hard
```

#Commit
``` bash
$ git commit
$ git commit -am "message"

$ git checkout [commit-id]
```

#Staged to modified
``` bash
$ git reset
$ git reset --hard 0ad5a7a6
```

#Push
``` bash
$ git push origin HEAD
```

#Pull
``` bash
$ git pull

$ git fetch origin
$ git merge origin/<branch_name>
```

#Log
``` bash
$ git log -p
```

#Checkout
``` bash
$ git checkout .

$ git checkout -
$ git checkout <commit_hash>

$ git checkout -b feature/xxx origin/feature/xxx
```

#Clean
``` bash
$ git clean -df
```

#Remote
``` bash
$ git remote -v
$ git remote add origin
$ git remote prune origin
```

#Branch
``` bash
$ git branch
$ git branch --delete [develop]
```

``` bash
#Extract Branch
$ git checkout develop

$ git branch feature/profile_management

$ git checkout feature/profile_management
```

``` bash
#Merge Branch
$ git checkout develop

$ git merge feature/profile_management

$ git branch --delete feature/profile_management
```

#Tag
``` bash
$ git tag --ist

$ git tag -a my_tag -m "crate tag v0.0.1"
$ git push origin <tag name> 

$ git tag --delete my_tag
$ git push --delete origin <tag name>
```


#Cherry Pick
``` bash
$ git cherry-pick [commit-id]
```