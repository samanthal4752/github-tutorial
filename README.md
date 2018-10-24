# GitHub Tutorial

_by Samantha Lui_

---
## Git vs. GitHub
**Git**-Keeps snapshots of the code and does not require github to function.

**Github**- Github requires git to save files/code. It stores code in the cloud.

---
## Initial Setup
**Making a Github account**-  
1. Log onto [Github.com](https://github.com/)
2. Make sure your github and c9 are connected. If it's not,go to your [c9](https://c9.io/) and go to the settings. Scroll to connected services and press connect when you see github.
3. Create a workspace dedicated to github
4. For auto save, you will have to go to the settings in c9 and click preferences. After that, you have to click Experimental then Files. You should see Auto-Focus and switch it to **On focus change**. If you don't want it to auto save and do it manually, You can use ctrl+S to save the changes.  

**SSH Key**-   
Your SSH key is used to clone files. You will have to input your SSH in the URL part of ```git clone URL```.
Your SSH key will look something like: git@github.com:YOURUSERNAME/FILE-NAME.git

---
## Repository Setup
1. Log into your [github](https://github.com) account  
2. Click on ```New repository```
3. Make a file with the **same** name as the one in c9
4. **Init**-With ```Git init``` you are initializing git into your repository  
5. **Your first add**-Use ```git add file``` to add your files to the stage in order to be commited  
6. **Your first commit**-After adding your file, use ```git commit -m " "``` to save your changes to your repository. In the quotation marks, you have to write a message describing your file.  
7. Use ```git remote-v``` to show you where you sent your commits to after you git pushed
<!--You are missing some steps for 
---
## Workflow & Commands  
**Status** -```git status```is to see which files you staged in the commit 
You will see something like: ```On branch master
Your branch is ahead of 'origin/master' by 1 commit.```  
**Add** - ```git add .``` Adds the directory to the repository with the changes you made  
**Commit** - ```git commit -m "(INSERT MESSAGES)"``` Git commit is when you are saving all of the files in stage for the repository
You will see something like: ```[master 3defaca] github-tutorial
 1 file changed, 31 insertions(+), 6 deletions(-)```  
**Push** - ```git push``` is to publish your local commits   
You will see something like:```Warning: Permanently added 'github.com,192.30.253.113' (RSA) to the list of known hosts.
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.12 KiB | 1.12 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To github.com:samanthal4752/github-tutorial.git
   a2758df..3defaca  master -> master```  
---
## Rolling Back Changes  
**Undo edit** - To undo edit you will have to use ```git checkout file name```  
**Undo add** - To undo add you will have to ```git reset "FILE-NAME"```  
**Undo commit** -To undo commit you will have to ```git reset --soft HEAD~1```  
**Undo push** - To undo push you will have to ```git log``` then ```git revert```
---
## What to do if you did ```init``` wrong in a directory:   

If you used git init wrong in a directory, use ```rm -rf .git``` 

## How to completely remove a repository (local&remote)
To completely remove a repository, you have to use ```git remove rm```

---
## Collaboration
**Fork**- Forking is when you are copying the other person's remote and getting your own remote. After forking, you can push into your remote.   
**Clone**- Cloning then copies your remote onto your workspace using ```git clone URL```  
**Pull Request**- Pull request is notifing the person that what you pushed to their Github Repository. Before submitting a pull request, you have to fork and clone their repository to your local repository. Then after you made your changes, you have to commit and push onto your repository.   
**Pull**-```git pull``` bring changes from the remote repo down to your local repo.


