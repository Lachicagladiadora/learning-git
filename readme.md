# Learning Git 

---
## What is Git?
> _Version Control System (VSC)_  Software that allows to record all history of changes

---
## Terminology
**Repository** -> project tracked (history) by git

**Commit** -> change checked in git

**Branch** -> new paths taken by the project

**Clone** -> copy of project on local computer

**Fork** -> different project from one

---
## Workflow
![work flow](https://kelvinleong.github.io/resources/Git/git-workflow.jpg)

---
## Commands 
### General
`git add` / `git add -A` / `git add .`
`git commit` **fileName** / `git commit -m` **'fileName'** 
`git commit -am` **'fileName'**

### Modify commit / Status / All commits
`git commit --amend` 
`git status`
`git checkout` **'fileName'**
`git log` / `git log --oneline` / `git log --oneline --decorate`

### Compare
`git diff` / `git diff --staged` / `git diff` **hash1 _hash2_** 

### Undo 
`git reset` **'hash'** / `git reset --hard` **'hash'** / `git reset --soft` **'hash'**
`git revert` **HEAD** / `git revert --no-commit` **HEAD** / `git revert --continue