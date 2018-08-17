git-commands
============
A repo for convenient custom git commands and aliases.

## Usefull aliases
These are the aliases I use daily (more or less).

```
[alias]
  a = add
  co = checkout
  ci = commit
  st = status
  br = branch
  d = diff
  aci = !git add -A && git commit
  ps = push
  pu = pull
  m = merge
  acp = !"git add \"$1\" && git commit -m \"$2\" && git push && git status && :"
  delbr = !"git branch -d \"$1\" && git push origin --delete \"$1\" && git status && :"
  com = !"git checkout develop && git pull origin develop && git checkout \"$1\" && git merge develop && git status && :"
  ```

Most of them are pretty common (like a, ci, ci etc), but I also have som other aliases that i find quite usefull:

### `git acp <what_to_add> <commit_message>`
  * Command for adding files, make a commit and push the current branch
  * **Usecase:** You want to add everything, commit it and push it to current branch

### `git delbr <branch_name>`
  * Commmand for deleting a branch locally and on origin
  * **Usecase:** You want to delete a branch locally and on origin

### `git com <branch_name>`
  * Command for checking out branch develop and pull latest changes, then checking out a specific branch and merge develop into it
  * **Usecase:** You are currently in a branch other than develop and want to merge in the latest

`acp, delbr and com` are also available as custom git commands. See [Usefull commands](#usefull-commands).


## Usefull commands
In addition to aliases I have created some custom commands (some I just have aliases for).

### How to use the commands
Add a folder cotaining the commands (the shell scripts) to your path. After you have done this you might need to restart your terminal. Then you should be able to use the commands like any other git commend, e.g `git delbr my-branch`

* `git acp <what_to_add> <commit_message>`
  * **Command for adding files, make a commit and push the current branch**
  * **Usecase:** You want to add everything, commit it and push it to current branch
* `git delbr <branch_name>`
  * **Commmand for deleting a branch locally and on origin**
  * **Usecase:** You want to delete a branch locally and on origin
* `git mpsdelbr <branch_name>`
  * **Commmand for merging, pushing and deleting (locally and on origin) a branch**
  * **Usecase:** You want to merge a branch in to your current branch, then push current branch and delete the merged branch locally and on origin
* `git com <branch_name>`
  * **Command for checking out branch develop and pull latest changes, then checking out a specific branch and merge develop into it**
  * **Usecase:** You are currently in a branch other than develop and want to merge in the latest changes from branch develop
