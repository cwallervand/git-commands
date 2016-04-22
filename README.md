git-commands
============
A repo for convenient custom git commands.

## How to use the commands ##
Add the folder cotaining the commands to your path. After you have done this you might need to restart your terminal. Then you should be able to use the commands.

## Available commands ##
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
