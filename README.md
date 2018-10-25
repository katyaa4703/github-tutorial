# GitHub Tutorial

_by Katya Anguisaca_

---
## Git vs. GitHub
  Git and Github are two differet things
 
 **Git**: Is the version control that keeps snapshots of the code. It does not require github. In other words, git is a command line tool.
  
 **Github**:Is the service for projects that use git. Github stores code in the cloud, visually tracks changes in the 
 code, easily collaborates on files and requires 'git'.
  

---
## Initial Setup
 The Initial Steup consists of creating a github account if you have not already done so and the SSH Key setup.
 
 **Github Account Setup**:
 * Open up your browser
 * Type in "github create account" and press the first result you see.  [Github.com](https://github.com/join)
 * Once you have clicked on the websit begin creating your account
 * Create your username
 * Then type in an email adress to associate it with your account
 * Create a password that you will remember or write it down
 * Then click on "create account"
 * Once you have created your own personal account go ahead and follow the instructions presented by gihub. Choose your plan and then tailor your experience
 
The setup of an SSH Key is very important. By having an SSH key you can connect and authenticate to remote servers and services. By having and SSH key, you can connect 
to Github without needing your username or password. SSH keys come in pairs. One of the pairs is a public key and the other one is a private key. The public key gets shared with services like Github and the private key that ges stored in 
your computer only. If the key matches then you are granted acces. 
  
 **SSH Key Setup** :
 * go into your github account
 * On the top-right corner press on your profile icon and then press on settings
 * When you see the left side bar press press on SSH and GPG
 * Then create a new SSH key (you shouls see the icon "new SSH key/Press on that")
 * Title your new SSH key "cloud9"
 * Then switch to your cloud9 tab. Once you have switched to your cloud9 tab, press on the top right and press on gear icon
 * Then press SSH keys tab 
 * Copy and paste the 2nd SSH key int github (private). It should beging with ssh-rsa
 * Then add SSH key. Go to cloud9  
 * Open github-learning IDE
 * In the workspace put in " ssh -T git@github.com"
 * Once ths is done, you will see "Hi <your username>! You've succesfully authenticated but github does not provie shell acces."


---
## Repository Setup
 There are a few steps to follow yo setup your repository. The steps are the following:
 1. In cloud 9, open up a new terminal
 2. Cd into workspace (cd ~/workspce)
 3. Make a new directory called first-repo (mkdir first-repo)
 4. Go into the new directory that was made (cd first-repo)
 5. Then, git init 
 6. Once git init has been added to the terminal, you can add a README file by using touch (touch README.md)
 7. Then, open the README file and type in "This is my first repo"
 8. Once this has been done, save, add the changes, and commit
 9. When you commit, type in the message "create readme". The full command should look like "git commit -m "create readme"
 10. In order to continue, we need to have a remote to push this into
 11. Now, go to your github account
 12. Press on the icon that has a "+" with a down arrow next to it on the top right corner.
 13. Then click on "New Repository"
 14. Name your repository the same way you named your directory in cloud 9 (first-repo). The names always have to match!
 15. Now, click on create repository. If you were asked to verify your email do it. However, if you were asked but didn't do it don't worry about it.
 16. Make sure that you have SSH selected
 17. Scroll down to the section that says "..or push an existing repository to the command line"
 18. Copy "git remote add origin..." and "git push..." one at a time to your terminal in your firs-repo README file (where the rest of the code is)
 19. Once this is all done and you have done the remote command, refresh github.
 20. You should know see your changes!


---
## Workflow & Commands
 There are many commands that can be used to create code in github. Such commands include: 
 * **git status:**
    git status is a command that allows you to track all the work/code you have been doing so far. It's a command that allows you to see which files have been edited since the last commit. These files will appear in red. In addition to this, this command will allow you to see the files that are staged for the commit. The files that are staged for the commit will appear in green.
* **git add:** 
    git add is a command used to add the current/entire directory. This command adds all the files that have changed. However, this only works for new or modified files. It will not add to the stage any deleted or renamed files. For example if you want to add a file called "chocolate.txt" in a directory you would type in _"git add chocolate.text"_. Since git add does not add any deleted or renamed files to the stage, you will be able to use _"git add --all"_ to include all changes. 
* **git commit:**
    git commit is a command that takes a snapshot of the files on the stage. When writing this command, there is a message that needs to be typed. The message should be present-tense and describe what was modified in this snapsht (create HTML Template)(take a picture). For example, if you have made made changes in the section called "apples", your commit command should look something like _'git commit -m "update apple section"_.
* **git push:**
    git push is a command that sends the commits from the local repo to the remote repo (up to the cloud :Github). For example, in order for the commits to be sent from the local repo to the remote repo you being by typing _"git add ."_ From here, you type in "_git status_" to see what files have been edited. Since you have made changes and already typed in the command "_git add ._" you see the files that are staged for the commit and they will appear in green. Once you see that the files are staged for the commit, you commit by addig a message which will look like "_git commit -m "type message here"_".Once everything has been commited, you then do "_git push_" to send he commits o the remote repo. 
* **git remote:**
   A remote in git is seen as a bookmark for other repositories from which the user may wish to pull or push the code. The repository that was bookmarked may be on your local computer at a different folder, in a remote server or it might be the repository itself. There are two git commands that consist of _'git remote_'. The first command that consists of git remote is 'git remote add origin URL'. This command allows you to add the remote repo as opposed to editing or removing an existing one. 
   The second command that consists of '_git remote_'is known ass '_git remote -v_'. This command allows the user to set up a connection between the current repository and the external one (the one that lives on github)




---
## Rolling Back Changes
 While creating code, there will be code that you might want to undo or revise. There will be certain commands that you will want to undo. For example:
 * To undo "git edit" you will have to type in "git checkout -- filename"
 * To undo "git add " you will have to type in "git reset HEAD-1 filename"
 * To undo "git push" you will have to type in "git push origin --delete <branch_name".
 * To undo "git commit" you will have to type in " git reset HEAD^".
---
## Error Handling
  During the process of coding, many errors can be made. Such errors can include that you `init` in the wrong directory or you might want to completely remove a repository. If you ever 
  init in the wrong directory, you can simply just type : **'rm -rf .git'**
