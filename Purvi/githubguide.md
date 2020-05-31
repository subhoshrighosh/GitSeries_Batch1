#How github works, cloning, forking, making PR’s, opening issues?
#Git:
* Git is a high quality version control system.
* Git can be easily installed and maintained on our local system and give a complete record on our local system and give a complete record of our ongoing programming versions.
*It is a command line tool that requires an interface to interact with the world . 
*It stores and catalogs changes in code in a repository.
##GitHub:
_GitHub is a best platform to explore new things. GitHub is a best way to connect with the peopl across world and learn new things from them._
##Step1:
** GitHub Forking:**
* after creating own github account we can take someone else data through forking.
* Forking is the best way to extract others data and start working on it.
##Steps to Fork other's data:
* Fork this repo owned by Earth Lab into your GitHub account.
##Step2:
** GitHub Cloning:**
* Once we fork someone's data next step is of cloning. It simply means download the zip file and extract into our desktop.
* After cloning we can create our own directory and add files into it to make it more attractful.
##How to clone
* Write git clone https://gitseries.com
*Clone the fork of your repo, so you can edit the contents locally
* Make edits to your local cloned copy of the repo on your computer
*add, commit and push those edits back to your fork on GitHub
##Step3:
* After adding our own content next step is to send Personal Request.
*PR can be seen as informing others about the changes that we have made in a project or in a branch when we pull request that means we
are requesting others to view the cahnges that we have made and merge it with the master branch.
*Suggest the changes that you made, to be added to the Earth Lab central repo using a pull request.
##Step 4:
** Opening Issues **
* Issues can be used to keep track of bugs, enhancements, or other requests. 
*Any GitHub Enterprise user can create an issue in a public repository where issues have not been disabled. 
*You can open a new issue based on code from an existing pull request.
##Steps to create an issue
*On GitHub Enterprise, navigate to the main page of the repository.
*Under your repository name, click  Issues.
*Click New issue
*If there are multiple issue types, click Get started next to the type of issue you'd like to open.
*ype a title and description for your issue.
*When you're finished, click Submit new issue.
##Mege Conflicts:
*A merge conflict is an event that occurs when Git is unable to automatically resolve differences in code between two commits.
*When all the changes in the code occur on different lines or in different files, Git will successfully merge commits without your help.
# Steps to Resolve Merge Conflict:
*Under your repository name, click  Pull requests.
*In the "Pull Requests" list, click the pull request with a merge conflict that you'd like to resolve.
*Near the bottom of your pull request, click Resolve conflicts.
*Decide if you want to keep only your branch's changes, keep only the other branch's changes, or make a brand new change, which may incorporate changes from both branches. 
*Delete the conflict markers <<<<<<<, =======, >>>>>>> and make the changes you want in the final merge.
*If you have more than one merge conflict in your file, scroll down to the next set of conflict markers and repeat steps four and five to resolve your merge conflict.
*Once you've resolved all the conflicts in the file, click Mark as resolved.
*If you have more than one file with a conflict, select the next file you want to edit on the left side of the page under "conflicting files" and repeat steps four through seven until you've resolved all of your pull request's merge conflicts.
*Once you've resolved all your merge conflicts, click Commit merge. This merges the entire base branch into your head branch.
*If prompted, review the branch that you are committing to.

*If the head branch is the default branch of the repository, you can choose either to update this branch with the changes you made to resolve the conflict, or to create a new branch and use this as the head branch of the pull request.
*If the head branch of your pull request is protected you must create a new branch. You won't get the option to update the protected branch.
*Click Create branch and update my pull request or I understand, continue updating BRANCH. The button text corresponds to the action you are performing.
*To merge your pull request, click Merge pull request. For more information about other pull request merge options, see "Merging a pull request.
## Branches in GitHub
* Branch is basically  a part or version of repo. A single repo can have multiple branches that can be merged into one as well.
*By default : Master branch e.g. if we are working on project under master branch and suddenly we create another branch names X and continue the project 
, we can go back to that instance where we created branch i.e working on branch will not affect other branches thus helping in creatig and accessing the different versions of project.
## Can we delete the master branch?
* No we cannot delete the Master Branch as soon as we use command "git init", Master branch gets activated by default.
## How can we delete a branch?
* Use Command: git branch -d<name of the branch>
#What is the difference between git branch -d and git branch -D?
* The -d option will delete the branch only if it has already been pushed and merged with the remote branch.
* We use -D instead if we want to force the branch to be deleted ,even if it has not been pushed or merged yet.
* The branch will now be deleted locally.
 
