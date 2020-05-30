# Basic guide to git and github! 📔
**1.What are git and github ?**

**Git**- Git is a type of version control system that makes it easier to track changes to files or in the source code. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. It is a program installed in a system. 
Its current maintainer since 2005 is Junio Hamano. As with most other distributed version-control systems, and unlike most client–server systems, every Git directory on every computer is a full-fledged repository with complete history and full version-tracking abilities, independent of network access or a central server.

**GitHub**- It provides hosting for software development version control using Git. It allows us to create remote repository on website and provides a platform to bring teams together.
GitHub accounts are commonly used to host open source projects.


**2.How github work ?**

Git workflow has four fundamental stage-

 Git workflow has 4 fundamental stages: 
  i.   Workspace: Working Directory 
  ii.  Index (Stage): It is used as a staging area between working directory and your repository
  iii. Local Repository is the one on which we will make local changes, generally Local Repository is on our computer.
  iv.  Remote Repository is the one of the server.


**Forking**
Forking means creating a personal copy from others project and it help us to modify and make changes in it without affecting the original content. 

**steps to fork the Repo:-**

Forking a repository is a simple two-step process. Fork an example repository

step1.On GitHub, navigate to the octocat/Spoon-Knife repository.

step2.In the top-right corner of the page, click Fork.

**Cloning**
When you create a new repository on GitHub, it exists as a remote location where your project is stored. You can clone your repository to create a local copy on your computer so that you can sync between both the local and remote locations of the project.

**Steps to create a local clone of your fork:-**

step1.On GitHub, navigate to your fork of the Spoon-Knife repository.

step2.Under the repository name, click Clone or download.

step3.To clone the repository using HTTPS

step4.Open Git Bash.

step5.Change the current working directory to the location where you want the cloned directory.

step6.Type git clone, and then paste the URL you copied earlier.

step7.Press Enter. Your local clone will be created.

**Making a PR**
PR stands for Pull Request.When you make local code changes and then submit those changes to a remote project maintainer for review before those changes are implemented, or merged.
This is called a pull request; you are requesting that someone reviews and approves your changes before they become final.


If you want to contribute in existing repository then fork that repository first and do some changes in tha repository's any section even if you change documentation of that repository's code and you think it should be in master repository of main repository than pull request it to main repository so that master can see and made changes to the repository.

**Steps to create a pull request:-**

step1.On GitHub, navigate to the main page of the repository.

step2.In the "Branch" menu, choose the branch that contains your commits.

step3.To the right of the Branch menu, click New pull request.

step4.Use the base branch dropdown menu to select the branch you'd like to merge your changes into, then use the compare branch drop-down menu to choose the topic branch you made your changes in.

step5.Type a title and description for your pull request.

step6.To create a pull request that is ready for review, click Create Pull Request.

**Issue**
Issues can be used to keep track of bugs, enhancements, or other requests.

**Steps to create an issue:-**

step1.On GitHub, navigate to the main page of the repository.

step2.Under your repository name, click Issues.

step3.Click New issue.

step4.If there are multiple issue types, click Get started next to the type of issue you'd like to open.

step5.Type a title and description for your issue.

step6.When you're finished, click Submit new issue.

## Basics commands used in git
**1. git config**

Usage : To set your user name and email in the main configuration file.

How to : To check your name and email type in git config --global user.name and git config --global user.email. And to set your new email or name git config --global user.name = “Ashwini Kumar” and git config -- global user.email = “ashwinikumar623@gmail.com”

**2. git init**

Usage : To initialise a git repository for a new or existing project.

How to : git init in the root of your project directory.

**3. git clone :**
Usage : To copy a git repository from remote source, also sets the remote to original source so that you can pull again.

How to : git clone <:clone git url:>

**4. git status**

Usage : To check the status of files you’ve changed in your working directory, i.e, what all has changed since your last commit.

How to : git status in your working directory. lists out all the files that have been changed.

**5. git add**

Usage : adds changes to stage/index in your working directory.

How to : git add .

**6. git commit**

Usage : commits your changes and sets it to new commit object for your remote.

How to : git commit -m”sweet little commit message”

**7. git push/git pull**

Usage : Push or Pull your changes to remote. If you have added and committed your changes and you want to push them. Or if your remote has updated and you want those latest changes.

How to : git pull <:remote:> <:branch:> and git push <:remote:> <:branch:>

**8. git branch **
Usage : Lists out all the branches.

How to : git branch or git branch -a to list all the remote branches as well.

**9. git checkout**

Usage : Switch to different branches

How to : git checkout <:branch:> or_git checkout -b <:branch:> if you want to create and switch to a new branch.

**10. git merge**

Usage : Merge two branches you were working on.

How to : Switch to branch you want to merge everything in. git merge <:branch_you_want_to_merge:>
