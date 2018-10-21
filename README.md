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
 The Initial Steup consists of creating a github account if you have not already dne so and the SSH Key setup.
 
 **Github Accoutn Setup**:
 * Open up your browser
 * Type in "github create account" and press the first result you see.  [Github.com](https://github.com/join)
 * Once you have clicked on the websit begin creating your account
 * Create your username
 * Then type in an email adress to associate it with your account
 * Create a password that you will remember or write it down
 * Then click on "create account"
 * Once you have created your own personal account go ahead and follow the instructions presented by gihub. Choose your plan and then tailor your experience
 * **SSH Key Setup** :


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
 There are many commands that can be used to create code in github.Such commands include: 
 * **git status:**
    git status is a command that allows you to track all the work/code you have been doing so far. It's a command that allows you to see which files have been edited since the last commit. These files will appear in red. In addition to this, this command will allow you to see the files that are staged for the commit. The files that are staged for the commit will appear in green.
* **git add:** 
    git add is a command used to add the current/entire directory. This command adds all the files that have changed. However, this only works for new or modified files. It will not add to the stage any deleted or renamed files. For example if you want to add a file called "chocolate.txt" in a directory you would type in _"git add chocolate.text"_. Since git add does not add any deleted or renamed files to the stage, you will be able to use _"git add --all"_ to include all changes. 
* **git commit:**
    git commit is a command that takes a snapshot of the files on the stage. When writing this command, there is a essage that needs to be typed. The message should be present-tense and describe what was modified in this snapsht (create HTML Template)(take a picture). For example, if you have made made changes in the section called "apples", your commit command should look something like _'git commit -m "update apple section"_.
* **git push**
    git push is a command that sends the commits from the local repo to the remote repo (up to the cloud :Github). For example, in order for the commits to be sent from the local repo to the remote repo you being by typing _"git add ."_ From here, you type in "_git status_" to see what files have been edited. Since you have made changes and already typed in the command "_git add ._" you see the files that are staged for the commit and they will appear in green. Once you see that the files are staged for the commit, you commit by addig a message which will look like "_git commit -m "type message here"_".Once everything has been commited, you then do "_git push_" to send he commits o the remote repo. 
    



---
## Rolling Back Changes