---
title: Basic Git Commands
subtitle: Some useful commands for git 
summary: This post contains all the basic initial commands for initializing or publishing a repo 
# description: 
# slug: basic-git-commands
# authors:
#     - Ukant Jadia

draft: false
date: 2023-12-30T14:15:59+05:30
lastmod: 


featured: true
projects: []

image:
    # caption: 'Image credit: Ukant'
    focal_point: ''
    placement: 1
    preview_only: false

categories:
    - Version Control System-VCS
tags:
    - Git
    - Basics
    - Linux
---


# what you should do in git
1. git init -b main 
2. git remote add origin <repo_link>
3. git remote -v


----
```bash
cd to the root file of the project
echo "+ Project " >> README.md
git init
git add .
git commit -m "README"
git branch -M Main
git remote add origin <repo_link> 
git push -u origin Main
```
----
+ pushing an existing repo from cli
git remote add origin https://github.com/UserCtf777/Inkdrop.git
git branch -M Main
git push -u origin Main



--- 
after clonning any repo it have the address of origin, simply you cannot add your repo url for backup/project/ICR
for that you have to change the origin url follow the following command

+ to check the origin url try the remote verbose
git remote -v

+ to change the remote origin try
git remote set-url origin <repo_url>



---
+ new error found
+ sometimes when we clone the repo we use depth=1 to remove it's history 
+ this give the error during pushing it to other origin 
+ error looks like 
+          ![remote rejected] Main -> Main (shallow update not allowed)
+	    error: failed to push some refs to

+ to solve this try 
git remote set-url <old_url>
git fetch --unshallow old 
1. git init -b main 
2. git remote add origin <repo_link>
3. git remote -v


----

cd to the root file of the project
echo "+ Project " >> README.md
git init
git add .
git commit -m "README"
git branch -M Main
git remote add origin <repo_link> 
git push -u origin Main

----
+ pushing an existing repo from cli
git remote add origin https://github.com/UserCtf777/Inkdrop.git
git branch -M Main
git push -u origin Main



--- 
after clonning any repo it have the address of origin, simply you cannot add your repo url for backup/project/ICR
for that you have to change the origin url follow the following command

+ to check the origin url try the remote verbose
git remote -v

+ to change the remote origin try
git remote set-url origin <repo_url>



---
+ new error found
+ sometimes when we clone the repo we use depth=1 to remove it's history 
+ this give the error during pushing it to other origin 
+ error looks like 
+          ![remote rejected] Main -> Main (shallow update not allowed)
+	    error: failed to push some refs to

+ to solve this try 
git remote set-url <old_url>
git fetch --unshallow old 
+!/bin/bash

cd ~/work/obs/Obsidian 

git add .
git commit -m 'daily update'
git push 

+!/bin/bash

+ to make dir work as git repo
git init

+ to check the changes
git status 

+ to sort/simplify the changes
git add .

+ git log shows the log of all commit done
git log

+ restore to discard the changes
git restore .

+ to commit the changes [with '-m' for successful commit/{-m => metadata of changes}]
git commit -m "daily update"

+ git push to add new file to the repo
git push 



+ command to add remote repo / it skip the authentication part during git push
git remote add origin git@github.com:UserCtf777/Obsidian.git
git branch -M master
git push -m origin master

+ To solve the conflicts during rebasing 
git rebase --continue + fix conflicts and run this
git rebase --skip + to skip this patch/changes
git rebase --abort + to checkout the original branch 

+ When we have unresolved conflicts before merging or having error related to add
git fetch + to gain the latest changes from server
git merge origin master + to give a try to automatice merging
+ it will only work if branch has to merge something-- it can be checked with git status
git merge --abort  + the unresolved conflicts will be cleared off

+ to edit the conflicts
git rebase --edit-todo 
git rebase --continue

+ if conflicts dosen't resolve then 
git rebase --abort 
+ it will give the path of unresolved files
+ if you know how to edit then resolve them 
+ OR you can remove that confict by
git rm <file>
+ if nothing is ahppening you can skip the commit wiht
git rebase --skip
