# GitHub Tutorial

_by Jessica Paez_

---
## Git vs. GitHub
* Git's independent of github because it's a tool to have save code.   
* Github is dependent of git, because it saves different files of coding in the cloud, saves changes made in the code, and allows collaboration of files between individuals.


---
## Initial Setup
* Allows you to be secured for authorization for your username/password. When you connect a GitHub repository to Git it'll have to be authenticate with GitHub. SSH allows you to authorize Github. This helps you push things into Git Hub without your pawssword, so it's quicker and more efficient.  
   

**To make a GitHub account :** 
1. You go to the website of GitHub and press the sign up option.
2. Creat your peronal account with your information, aso in an username, email and password.
3. Review the policy to then create the account.
4. You then choose a plan that can be free or paid.
5. You've created your account.  


 **In order to make the SSH key beween GitHub and c9 it's:**
1. Go to GitHub and in the top right corner it has a profile icon then it you go to settings 
2. On the left side bar there's SSH and GPG.
3. Then you chose the "New SSH key"
4. You then title it to be "cloud 9"
5. Making the key  
    Go to the could 9 tab and on the top right the gera icon.  
    Go to the SSH key tabs to then have the second SSH key be placed into GitHub by copy and pasting it, and it starts with "ssh-rsa".  
You add the SSH key. 
6. You open cloud 9 and then you open git hub learning IDE  
       In the workspace you put ssh -T git@github.com  
       You then recieve "Hi < your username>! You've successfully authenticated, but GitHub does not provide shell access._"
 
---


## Repository Setup
1. You go into c9 and make sure you're in the workspace by "cd ~/workspace"
2. You then make the directory by "mkdir first-repo"
3. You then go into the directory with " cd first-repo"
4. You then intialize git with "git init"  `**'Git init':**` Its a version control that allows you to create an empty git repository. This then appears as a git. directory, and  it allows you to have a git repository that's existing be reinitialize. If this was placed in the wrong directory you go into that directory that you misplaced the "git init", and this is removed by "rm -rf .git".
5. You go into GitHub and press the right top corner where the plus sign appears. To the "New repository".
6. This "New repository" is then names "first-repo". The names always have to match.
7. Then you create the repository and its done.


---
## Workflow & Commands
* **`Git status`:**   
     Allows you to keep track on your coding and the changes you've done. The changes that have been made by editing are in red, and green are the one's that you have staged and commited.
* **`Git add`:**   
     Allows you to have changes be placed into the staging area. This has it tracked and prepares it to then be committed. In order to add just the current directory on it `git .` and if it's been changed or modify. In order to add all the files even those that have been deleted or renamed you use `git add --all`. 
* **`Git commit`:**   
     Is the action of saving the changes from the staging area into the respitory, and GitHub is the repository. You leave a commit using `git commit -m "message"`. It’s a snapshot’ of the files on stage. Message  is in -present tense and it describes what was modified in this snapshot.
* **`Git push`:**   
    Is to have the changes you've made be saved to your remote repository from your local branch. Git push -u pushing it to the cloud somwheere the origin (nickname) where it’s being send to master (location and what branch).
* **`Git init`:**   
 Its a version control that allows you to create an empty git repository. This then appears as a git. directory, and  
 it allows you to have a git repository that's existing be reinitialize. If this was placed in the wrong directory you go into that directory that you misplaced the `git init`, and this is removed by `rm -rf .git`.

 
---
## Rolling Back Changes
* Undo edit is used by `git checkout --filename`. It undos the changes made in a file.
* Undo git add by using `git reset HEAD filename`. It was put on the stage, it can be removed.
* Undo git commit with `git reset --soft HEAD~1`. It was saved from the stage, it now can be removed.
* Undo git push with `git reset --hard HEAD~1`. It removes whats been placed in the remote.


---
## Collaboration 

* `Git clone` - If you clone someone else repository, you have a local copy of their remote repository. However, you can't 'git push' into their remote because you don't have their permission.  

* Forking - you have a remote copy of someone else's remote repository. You can clone their remote and have permission to push to your remote.  

* Pull requests- After you've made changes and commits you push them to your remote. However the original persons remote recieves the pull request and decides to accept or deny the changes you've made and commited to the remote.  

* `Git pull` - Allows you to have your local copy of the repository be updated after you have merge your pull request. 