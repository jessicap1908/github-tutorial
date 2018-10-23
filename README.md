# GitHub Tutorial

_by Jessica Paez_

---
## Git vs. GitHub
* Git's independent of github because it's a tool to have save code.   
* Github is dependent of git, because it saves different files of coding in the cloud, saves changes made in the code, and allows collaboration of files between individuals.


---
## Initial Setup

* Allows you to be secured for authorization for your username/password. When you connect a GitHub  
repository to Git it'll have to be authenticate with GitHub. SSH allows you to authorize Github.  
This helps you push things into Git Hub without your pawssword, so it's quicker and more efficient.  
   
In order to make the SSH key beween GitHub and c9 it's:
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
4. You then intialize git with "git init"
5. You go into GitHub and press the right top corner where the plus sign appears. To the "New repository".
6. This "New repository" is then names "first-repo". The names always have to match.
7. Then you create the repository and its done.


---
## Workflow & Commands
* **Git init:** allows you to create an empty git respitory. This then appears as a git. directory and  
 it allows you to have a git repository that's existing be reinitialize.  
* **Git add:** allows you to have changes be placed into the staging area. This has it tracked and   
 prepares it to then be committed.  
* **Git commit:** is the action of saving the changes into the respitory and GitHub is the repository.
* **Git push:** is to have the changes you've made be saved to your remote repository from your local branch.


---
## Rolling Back Changes
* Undo edit is used by "git checkout --filename". So it has undo to be made, from the changes made in a file.
* Undo git add by using "git reset HEAD filename". So if it was put on the stage, it can be removed.
* Undo git commit with "git reset --soft HEAD~1". So if it was saved from the stage, it now can be removed.
* Undo git push with "git reset --hard HEAD~1"