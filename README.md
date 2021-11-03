# AG Grid Support Sessions - Git and Github tutorial
## Setting up 


`$ git init` 
creates a .git folder

`$ ls -la`
to see all files and folders (including hidden) 

`$ git add .`

`$ git commit -m "commit title" -m "commit description"`
this is only local

`$ git branch -M main`

`$ git remote add origin https://github.com/AhmedAGadir/git_session_prototype.git`
allows us to connect to a remote location online

`$ git push -u origin main`
-u stands for upstream and it just sets up a shortcut for `git push`



## Making changes

`$ git diff`
to see differences between your current project and your last commit 

`$ git diff branch_name`
to see difference between your branch and another branch




## Branching and Merging

`$ git branch`
to see what branch were on

`$ git checkout -b name_of_branch`
to create a new branch (make it descriptive e.g. feature-read-me-instructions)

`$ git checkout main`
to go back to the main branch


when merging you COULD 
`$ git branch main`
`$ git merge name_of_branch`

BUT the more common pattern is to:
- push the changes on the branch to github 
- make a Pull Request (PR) using the GUI. 
- pull the updated main onto your local machine
- delete the branch that was merged using `$ git branch -d name_of_branch`

 ### Merge conflicts

- merge the main version locally into your branch
- solve merge conflicts in your text editor 
- push to github and make a PR 
- switch to main branch, pull, delete temporary branch



## Revert 

`$ git reset`
`$ git reset name_of_file_to_unstage`
to undo `git add`

`$ git reset HEAD~1`
to go back 1 commit 

`$ git log` 
and then copy the commit 
`$ git reset HASH_OF_COMMIT`
`$ git reset --hard HASH_OF_COMMIT`
to revert back further than one commit



## Forking
fork github repos online so that you can be free to do your own thing




