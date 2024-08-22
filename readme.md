# Learning Git 

---
## What is Git?
> _Version Control System (VSC)_  Software that allows to record all history of changes

-  Does not require internet
- Is fast
- GIT create copies from original project
- DATA INTEGRITY: Clones created from data; therefore the data is the equal, clean and not corrupted.

---
## Terminology
1. GIT(VCS- Version Control System) ->  Software which save changes history
2. REPOSITORY ->  Project followed for GIT, project which have history in GIT
3. COMMIT ->  Change registered in GIT, the change have a message
4. BRANCH -> New alternative trail for project
5. CLONE ->  Project copied in local PC
6. FORK -> Different project from once project

---
## Workflow
![work flow](https://kelvinleong.github.io/resources/Git/git-workflow.jpg)

---
## Commands 
### Config first time
- name -> `git config --global user.name <"John Doe">`
- email -> `git config --global user.email <johndoe@example.com>`
- editor -> `git config --global core.editor <editor>`
- default branch Name -> `git config --global init.defaultBranch main`

SHOW CONFIG: `git config --list`

### General
- `git add` / `git add -A` / `git add .`
- `git commit` **fileName** / `git commit -m` **'fileName'** 
- `git commit -am` **'fileName'**

### Modify commit / Status / All commits
- `git commit --amend` 
- `git status`
- `git checkout` **'fileName'**
- `git log` / `git log --oneline` / `git log --oneline --decorate`

### Compare
- `git diff` / `git diff --staged` / `git diff` **hash1 _hash2_** 

### Undo 
- `git reset` **'hash'** / `git reset --hard` **'hash'** / `git reset --soft` **'hash'**
- `git revert` **HEAD** / `git revert --no-commit` **HEAD** / `git revert --continue

### For staged
-  `git stash` -> save work in the stage
-  `git stash list` -> show all files saved in the stage
-  `git stash apply` -> open the last file from stage
-  `git stash drop` -> delete stage contain
-  `git stash pop` -> take out the last thing that was saved

### Branches
- `git branch` -> show the branches
- `git branch <feature>` -> create a new branch
- `git checkout <feature>` -> change of branch with pointer
- `git checkout -b <feature>` -> create a branch, move local changes and move the pointer to that branch
- `git branch -m <actualBranchName> <newBranchName>` 
- `git branch -d <branchName>` -> delete branch
- `git branch -D <branchName>` -> force delete branch