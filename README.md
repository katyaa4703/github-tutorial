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



---
## Rolling Back Changes