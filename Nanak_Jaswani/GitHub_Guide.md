What are git and github?
First of all, GitHub is not git.
Many people understandably confuse the two.GitHub is a website for hosting projects that use git.
Git was developed in 2005 by Linus Torvalds, the famous creator of the Linux operating system kernel.
It is open-source,free and distributed version control system(VCS).that makes it easier to track changes to files.
Git has trunk based development in it which involoves branches in the repository in which we can create a new branch
even while working with current branch and also we can merge the new branch with the master branch if required at any 
point.GitHub is a website on which we wan can upload projects. GitHub is a file sharing service to collaborate with different people.

How github work

Git workflow has four fundamental stage-
a. Workspace: working directory
b. Index(stage) :It is used as staging area between working directory and your repository
c. Local repository is the one on which we will make local changes, generally Local repository is on our computer. 
d. Remote repository is one of the server. 

github is an online version control system.
It is based on Git and provides some other additional features of its own.
Github lets you store your code remotely known as repositories,
which you can access from anywhere or work together with your team members on a certain project.

Forking

Forking in GitHub is a process of creating a copy of a complete repository 
to the user's GitHub Account from another account. When a user forks a repository,
all the files in the repository are automatically copied to the user's account
on GitHub and it feels like the user's own repository.

steps to fork the repo

Forking a repository is a simple two-step process.
Fork an example repository

1.On GitHub, navigate to the octocat/Spoon-Knife repository.
2.In the top-right corner of the page, click Fork.

Cloning

Cloning basically means you want to get a local copy of the code present 
in the repository. After cloning you can then do whatever changes you 
like in the code and then you can pull the changes back to the repository.

Steps to create a local clone of your fork-
1.On GitHub, navigate to your fork of the Spoon-Knife repository.
2.Under the repository name, click Clone or download.
3.To clone the repository using HTTPS
4.Open Git Bash.
5.Change the current working directory to the location where you want the cloned directory.
6.Type git clone, and then paste the URL you copied earlier.
7.Ex-$ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
8.Press Enter. Your local clone will be created.

Making a PR
A pull request is submitted when you’ve worked on some code
from a particular branch and want to inform the others of the changes you’ve made.

If you want to contribute in existing repository then fork that repository first 
and do some changes in tha repository's any section even if you change documentation
of that repository's code and you think it should be in master repository of 
main repository than pull request it to main repository so that master
can see and made changes to the repository.

Creating the pull request

1.On GitHub, navigate to the main page of the repository.
2.In the "Branch" menu, choose the branch that contains your commits.
3.To the right of the Branch menu, click New pull request.
4.Use the base branch dropdown menu to select the branch you'd like to merge your changes into,
then use the compare branch drop-down menu to choose the topic branch you made your changes in.
5.Type a title and description for your pull request.
6.To create a pull request that is ready for review, click Create Pull Request. 

Issue 
Issues can be used to keep track of bugs, enhancements, or other requests.

Creating an issue
1.On GitHub, navigate to the main page of the repository.
2.Under your repository name, click  Issues.
3.Click New issue.
4.If there are multiple issue types, click Get started next to the type of issue you'd like to open.
5.Type a title and description for your issue.
6.When you're finished, click Submit new issue.


10 Basics commands used in git

1) git config
Utility : To set your user name and email in the main configuration file.
How to : To check your name and email type in git config --global
user.name and git config --global user.email. And to set your new email or
name git config --global user.name = “Dhruv Nenwani” and git config --
global user.email = “nendhruv@gmail.com”

2) git init
Utility : To initialise a git repository for a new or existing project.
How to : git init in the root of your project directory.

3) git clone
Utility : To copy a git repository from remote source, also sets the remote to 
original source so that you can pull again.
How to : git clone <:clone git url:>

4) git status
Utility : To check the status of files you’ve changed in your working directory, i.e, what all has changed since your last commit.
How to : git status in your working directory. lists out all the files that have been changed.

5) git add
Utility : adds changes to stage/index in your working directory.
How to : git add .

6) git commit
Utility : commits your changes and sets it to new commit object for your remote.
How to : git commit -m”sweet little commit message”

7) git push/git pull
Utility : Push or Pull your changes to remote. If you have added and committed your changes and you want to push them. Or if your remote has updated and you want those latest changes.
How to : git pull <:remote:> <:branch:> and git push <:remote:> <:branch:>

8) git branch
Utility : Lists out all the branches.
How to : git branch or git branch -a to list all the remote branches as well.

9) git checkout
Utility : Switch to different branches
How to : git checkout <:branch:> or **_git checkout -b <:branch:> if you want to create and switch to a new branch.

11) git merge
Utility : Merge two branches you were working on.
How to : Switch to branch you want to merge everything in. git merge <:branch_you_want_to_merge:>