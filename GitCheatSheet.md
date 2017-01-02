
Git CheatSheet makes easy to understand and use Git  with very straight forward commands. Very helpful for new Git users::::

Create Repository                                             |                  Git commands
--------------------------------------------------------------|---------------------------------------------------
Create New Repository                                         |      $ git init
Clone an existing Repository                                  |      $ git clone (Paste URL of existing Repository)

Add Changes                                                   |                   Git commands
--------------------------------------------------------------|----------------------------------------------------
Check status of working directory                             |      $ git status
Add current changed file in to next commit                    |      $ git add <paster file link>   
Add all current changes to the next commit                    |      $ git add . "here . indicates all changes"
Add some changes in specific file                             |      $ git add -p <file>

Commit Changes                                                |                   Git commands
--------------------------------------------------------------|-----------------------------------------------------
Commit all local changes                                      |      $ git commit -a "commit message"
Commit previously staged changes                              |      $ git commit
Commit changes with commit message                            |      $ git commit -m "commit message"

Commit History                                                |                   Git commands
--------------------------------------------------------------|-----------------------------------------------------
Show list of all commit                                       |      $ git log
Show changes for specific file                                |      $ git log -p <file>
How to track who, what & when changes done in <file>          |      $ git blame <file>

Publish & Integrate                                           |                   Git commands
--------------------------------------------------------------|------------------------------------------------------
Publish local changes                                         |      $ git push
Publish local changes on remote                               |      $ git push <remote> <branch>
Add new Remote Repository                                     |      $ git remote add <repo name> <url>
list all configured remotes                                   |      $ git remote -v
Download all changes from <remote> not Integrate into Head    |      $ git fetch <remote>
Update local Repository to the newest commit                  |      $ git pull <remote> <branch>

Branches, Merge & Rebase                                      |                    Git commands
--------------------------------------------------------------|--------------------------------------------------------
Switch branch                                                 |       $ git checkout <branch>
Create new Branch                                             |       $ git branch <new-branch>
Create new tracking branch based on remote branch             |       $ git checkout --track <remote/branch>
Merge branch in to current active branch                      |       $ git merge <branch>
Rebase your current Head onto <branch>                        |       $ git rebase <branch>

Discard all changes (undo)                                    |                     Git commands
--------------------------------------------------------------|----------------------------------------------------------
Discard local changes in specific file                        |       $ git checkout head <file>
Discard local changes in working directory                    |       $ git reset --hard Head
Revert commit <commit new contrary changes>                   |       $ git revert <commit>

Stashing & Cleaning                                           |                     Git commands
--------------------------------------------------------------|------------------------------------------------------------
switch branch without commit incomplete work                  |       $ git stash
To check stored stashes                                       |       $ git stash list
Reapply stash most recent                                     |       $ git stash apply
Reapply at specific stash                                     |       $ git stash apply stash@{stash number}
Stash untracked file                                          |       $ git stash -u
Create branch from stash                                      |       $ git stash branch <branch name>
