Team Members: Melody Wang, Rishika Thorat, Kevin Park, Darion Phan
Workflow: Forking WorkFlow

Description of Basic Git workflow: (as summarized by your group) 
The basic Git workflow works by allowing each collaborator to branch off of the original repository and make their changes. Once they are done, they can push back to the original repository, allowing every collaborator to see their changes. 

Description of Forking workflow: (as summarized by your group)
The forking workflow works by allowing each collaborator to have their own forked and local copy of the repository, allowing each person to work on a separate copy to prevent clashes. Through these local copies, developers create new branches for each feature they add. When they¿re finished working on the feature, they push the branch and create pull requests to the master branch.

Key Differences from basic workflow, and key use cases
The primary difference between forking and the basic workflow is the fact that forking has a different method on how they get shared. When sharing a forking workflow you have to pull it into the developer¿s local repository. With the basic workflow, it gets pushed to the main, shared repository. 

Link to your Git example repository: 
https://github.com/DHS-CP/CSAForkingWorkflowExample
Documentation of git commands used, and annotated sample sequence of commands used in creating your repository


For admin/master: 
git init
git add . 
git commit -m ¿your message here¿
git push

For collaborators:
MAKE A FORK OF THE ORIGINAL/MASTER REPO
git clone <link to forked repo>
git branch <name of branch>
git add .
git commit -m ¿your message here¿
git push

To update your forked repo/local repo after changes are made in the master:
git remote add upstream <link to original repo>
git fetch upstream
git checkout master
git rebase origin master
git push origin master
