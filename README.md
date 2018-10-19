# GitHub Tutorial

_by Felix_

---
## Git vs. GitHub

**Git** is a control version system that you can make changes to over time. You will be doing the command and writing files in your IDE not much difference.

**Github** is server online that act as a remote for what ever you push from your local.

---
## Initial Setup
1. Create a gihub account 
2. login to the github accont
3. link the account to you IDE with SSH key
4. youareset


---
## Repository Setup

1. Create a directory or go to the desinated location
2. Git init to create repository
3. create a file and the add > commit > push  
4. you are set 


---
## Workflow & Commands

git init- initialize directory  
git add - adds file to the stage  
git commit -takes a "screenshot" of your repository  
git clone -takes the repository of a certain thing and add it to you IDE  
git push- sent the commit to the remote  
git pull- pull the commit from a remote
git remote -u origin master create a bridge between the remote and the local
git status -check what is up
git remote -v  -check the status of linked remote
git diff - check what changes was made
git log -review preview commits
q - exit the any logs
rm -rf .git  - remove the bridge

---
## Rolling Back Changes
git checkout -- file - unedit  
git reset HEAD file - unadd  
git reset HEAD~1 uncommit and unadd  
git reset --soft HEAD file - uncommit  
git reset --hard HEAD file - uncommit unadd and unedit  
