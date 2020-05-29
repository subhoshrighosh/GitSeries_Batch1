# Summary of Git and Github!!


## This document is about Git and  Github  
- Features
- Working
- commands of Git Bash


## GIT :

- Git is a **distributed version-control system** for tracking changes in source code during software development.
- It is designed for coordinating work among programmers, but it can be used to track changes in any set of files.
- Its goals include speed,data integrity, and support for distributed, non-linear workflows.
- Git was created by **Linus Torvalds** in 2005 for development of the Linux kernel, with other kernel developers contributing to its initial development.
- As with most other distributed version-control systems, and unlike most client–server systems, every Git directory on every computer is a full-fledged repository with complete history and full version-tracking abilities, independent of network access or a central server.
- Git is free and open-source software distributed under the terms of the GNU **General Public License version 2**.


## GITHUB :

- Github is a website on which we can upload project
- GitHub is a development platform inspired by the way you work. From **open source** to **business**,you can host and review code,manage project.
- GitHub is a for-profit company that offers a cloud-based Git repository hosting service.
- GitHub’s interface is user-friendly enough so every coders can take advantage of Git. Without GitHub, using Git generally requires use of the command line.
- Through GitHub, you can share your code with others, giving them the power to make revisions or edits on your various Git branches.This makes it possible for entire teams to coordinate together on single project in real-time.

1. It supports all programming languages.
2. Provides secure cloud storage.
3. It provide collaboration.
4. Code review.
5. Graphical representation of branches.
6. social coding.



## GITBASH :

* Bash is an acronym for Bourne Again Shell.
* Git Bash is an application for Microsoft Windows environments which provides an emulation layer for a Git command line experience.

- Git commands which are being covered:

- git config
- git init
- git clone
- git add
- git commit
- git diff
- git reset
- git status
- git log
- git show
- git branch
- git checkout
- git merge
- git remote
- git push
- git pull



###  How Github Work :

Git workflow has four stage -
1. **Workspace :**  ( Working Directory ) Where we can have 3 states they are **Commited** ,**Modified** ,and **staged**.
2. **Index :**  Used as staging area in between working directory and your repository.( also known as stage ).
3. **Local Repository :**  ( Known as Head ) we make local changes .
4. **Remote Repository :**  It is server,typically a machine at 42 miles away.


 
#### Forking :

When one wanting to contribute to someone else’s project. Or maybe you’d like to use someone’s project as the starting point for your own. This process is known as **forking**.
Creating a **fork** is producing a personal copy of someone else’s project. Forks act as a sort of bridge between the original repository and your personal copy. 
A forked project also remain attatched to the original, allowing you to submit a pull request to the original author to update with your changes, ensuring you're always working off a rent or up-to-date codebase.


#### How to fork a repository :

- To fork the  repository, click the **Fork button** in the header of the repository.
- Sit back and watch the forking magic. When it’s finished, you’ll be taken to your copy of the repository.



#### Cloning :


Cloning a git repository means that you create a local copy of the code provided by developer. You can simply do it with a command line. To clone a repository means that you will download the whole code of the repository.


#### How to clone a repository :

You’ve successfully forked the repository, but so far, it only exists on GitHub. To be able to work on the project, you will need to clone it to your computer.
If you’re using GitHub Desktop, this process is a breeze. On your fork of repository , navigate over to the right hand side bar and click Clone or Download. 

- Some options are cloning with the command line :
1. Open Git Bash.
2. Change the current working directory to the location where you want the cloned directory.
3. Type git clone, and then paste the URL you copied earlier.
4. $ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.



#####  Pull Request:

**Pull Request :**  (PR) is a Github feature that allows users to collaborate better together. Usually in source control software there is a main branch that describes production in git it is the master branch.
One can create a feature branch and make changes there, then issue a PR to the master branch for someone else to review, approve or reject the changes and merge to the master branch eventually.



##### How to make PR ?

-  On Github navigate to main page of repository.

- In **Branch menu** ,choose the branch of in which you have made commit.

- Now press the **New pull request** button on your left-hand side of the page.

- You can modify the branch on the next screen. On either site you can select the appropriate repository from the drop-down menu and the appropriate branch.

- You should add in a title, a comment, and then press the **Create pull request** button.

- At this point, the maintainers of the original repository will decide whether or not to accept your pull request. They may ask for you to edit or revise your code prior to accepting the pull request.



###### Issues in Git :

**Issues :** Issues are a great way to keep track of tasks, enhancements, and bugs for your projects. They’re kind of like email—except they can be shared and discussed with the rest of your team. Most software projects have a bug tracker of some kind.
GitHub’s tracker is called Issues, and has its own section in every repository.



###### Creating Issues in git :

1. Clone the repository.
2. Select the Issue option.
3. Name the issue and write discription.
4. create the lable.
5. click **Create Issue** and the issue is created. 










