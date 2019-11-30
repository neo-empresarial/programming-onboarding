# Onboarding 

## Todo
- [ ] Learn git with [Gitit](https://github.com/jlord/git-it-electron)

## Git cheatsheet
Common console commands: 
 cd - change directory
 mkdir - make directory
 ls - view the files/folders in directory

NOTE: Exit VIM if needed ctrl + c then type :qa! and push enter
NOTE: If file is not in local repo, manually move the file into 
       the correct folder (outside of console)

--------------------------------------------
 Managing your Local Repo
--------------------------------------------
NOTE: If you need to hard reset your local repo to match 
       the remote master use the following commands:
```bash
git fetch origin
```bash
```git reset --hard origin/master
``` 
Undo the act of committing, leaving everything else intact:
```bash
git reset --soft HEAD^:
```
Undo the act of committing and everything you'd staged, 
but leave the work tree (your files intact):
```bash
git reset HEAD^
```
Completely undo it, throwing away all uncommitted changes,
 resetting everything to the previous commit:
```bash
git reset --hard HEAD^
``` 
--------------------------------------------  
 BEGIN WORKFLOW
-------------------------------------------- 
Clone the Repo to local machine:
```bash
git clone https://github.com/user_name/repo_name.git
``` 
Make sure the local master is up-to-date:
```bash
git pull origin master
```
Create new branch:
```bash
git banch branch_name
``` 
Move to branch:
```bash
git checkout branch_name
``` 
Navigate file structure as needed:
```bash
ls 
```bash
```cd folder_name
``` 
Add the files to the branch:
```bash
git add .
``` 
Verify file: 
```bash
git status
``` 
Commit the files:
```bash
git commit -m "comment"
``` 
Add branch and files to the Remote Repo:
```bash
git push -u origin branch_name
``` 
Go to the github website to manage pull request and merge. 
 
Switch back to local master so you can delete the local branch:
```bash
git checkout master
``` 
Delete local branch: 
```bash
git branch -d branch_name
``` OR 
```bash
git branch -D branch_name
``` 
 If you don't want to go to the website, you can merge your branch 
 to the master locally and push the new master to the remote repo:
 
Switch back to master branch:
```bash
git checkout master
``` 
Merge the branch with the local master:
```bash
git merge branch_name -m "comment"
``` 
Push the local master to the remote master:
```bash
git push origin master
``` 
Delete local branch: 
```bash
git branch -d branch_name
``` OR bash

```git branch -D branch_name```
