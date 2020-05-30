
# Git and GitHub

Git is distributed version control system.It is used to commit or save different versions of project with better understandable version names and its features.Git is program installed in system. Git comes with advantage of local repository .
GitHub is website which provide repository to store different versions of project.Github allow us to create remote repository on website.GitHub is built for collaboration,set up an organization to improve the way your team works together, and get access to more features.

**GitHub is so popular and used in most of the projects because:**
1.We can stire our all projects at one place
2.Acess anytime anywhere
3.Separate public and private repositories
4.Easy to contribute in project and easy for team work

**Platforms similar to GitHub are :**
Amazon code commit
GitBucket
Source Forge
Cloude source repositories

# Git workflow includes 4 stages #
1)Workspace(Working Directory)
2)Index(Stage)
3)Local Repository(Head)
4)Remote Repository

**Workflow for pushing file to remote repo is :**
Clone command creates a local copy of the repository in working directory.
Add command adds the file from working directory to the Index.
Then after commit, file get saved in local repo.
By using commit -a ,we can combinely do the work of add and commit.
After this by using Push command,we pushes file from local repo to remote repo.Once file get pushed in remote repo it can be viewed to all if its public repo and to specific authority if its private repo.

**Workflow to fetch files from remote repo is:**
Fetch : Fetch command is used to fetch file from remote repo to local repo.
Merge : Merge command is used to fetch file from local repo to working directory.
Pull : Pull command help us to fetch file directly from remote repo to working directory.


It is not possible to a git commit before git add . Because as per git workflow first we have to add file from working directory to index and then commit it into local repo.

git diff is used to know difference between status of files in repo after changes. git status is used along with git diff for analyzing file status more clearly.

We can use the commit message as blank.Because git provide facility as commit message for more understanding of each commit,Otherwise we can choose not to use this facility and keel commit message as blank.

# Git Bash
To use git command we have to use git bash.Git Bash is an application that adds an emulation layer on Microsoft Windows environments to use Git command-line experience. It is just like a package that installs some common bash utilities on a Windows operating system. It let us use all the Git features as well as most of the standard UNIX commands in a command-line interface on Windows. In git bash we can see internal process of every change we made in git file with comments given by git bash and also by using git commands.If we stuck in between ,we can take help by using git help command. git help command explains every git command and its use.

These are common Git commands used in various situations by me during each task:
*A. To start a working area*
   clone             Clone a repository into a new directory

*B. To work on the current change*
   add               Add file contents to the index
   rm                Remove files from the working tree and from the index

*C. To examine the history and state*
   diff              Show changes between commits, commit and working tree, etc
   log               Show commit logs
   status            Show the working tree status

*D. To grow, mark and tweak your common history*
   branch            List, create, or delete branches
   commit            Record changes to the repository
   merge             Join two or more development histories together
   reset             Reset current HEAD to the specified state
   switch            Switch branches

*E. To collaborate*
   fetch             Download objects and refs from another repository
   pull              Fetch from and integrate with another   repository or a local branch
   push              Update remote refs along with associated objects

# Branching 
Branches allow you to move back and forth between 'states' of a project. For instance, if you want to add a new page to your website you can create a new branch just for that page without affecting the main part of the project.A branch is an independent project link.Default branch is master,but we can change default branch. If we found two independent branches have compatible changes then it is useful to merge them.We can add as many branches we want and each one can be independent of each other.

Command for creating a new branch and moving to that branch from current branch is :**git checkout -b branchname** .
Command for deleting a branch is: **git branch -d branchname**.

# Fork
Fork is personal copy of someone else's projects.Fork acts as a sort of bridge between the original repository and iur personal copy.We can pull request to make contribution in other's project.But its solely depends on will of original programmer whether to make that changes or not.Still if for someone other if our changes are useful they can use it.
Clone means to copy our own repository to local computer to modify it.

**Steps to fork a Repo**
Go to the Repo which you want to fork.
click on fork button.

# Cloning
After forking you need to clone the forked repo to do changes inside that Repo.The git clone is a git command, which creates a clone/copy of an existing repository into a new directory.

**Steps for cloning:**
1.Click clone and download button
2.After clicking copy the link which it shows there.
3.Then open Git Bash.
4.Change the directory.
5.After Changing the directory type command git clone followed by link which you copied after clicking on clone and download button.

# Pull Request
PR or pull request are made to the owner of a forked repo so that he can see the changes done in the repo and based on that ,can approve the changes or not. If he approves the changes will be made to author's repo as well.

# Markdown Format
Text written in Markdown Format are more easily readable.We can use different tags for different styles of texts. Simple way to create markdown file is renaming any text file with .md extention. 

# Merge conflict
In every situation where work can be parallelized, work will eventually overlap. Sometimes two developers will change the same line of code in two different ways  in such a case git conflict occurs.
To remove merge conflict first we have to find where conflict has been occured.To find that we can search for some strange new additions such as following in file:
<<<<<<< HEAD
=======
>>>>>>> new branch to merge later

These new lines as "conflict dividers". The ======= line is the "center" of the conflict. All the content between the center and the <<<<<<< HEAD line is content that exists in the current branch master which the HEAD ref is pointing to. Alternatively all content between the center and >>>>>>> new_branch_to_merge_later is content that is present in our merging branch.

To resolve Merge Conflict we have to decide which part of conflict divider we want and which part we don't want. After removing unwanted part we can merge branches.
It is possible that there may be many merge conflict in file,so we have to search for all conflicts before merging.

**Difference between git branch -d and git branch -D is :**
git branch -d : This is a command used to delete a branch.The branch must be fully merged in its upstream branch or in HEAD 
git branch -D : This is a command use to delete a branch irrespective of its merged status

# Issue in Git
As Git and GitHub is also used for big project it is possible to have some issues in project.To assign particular domain issue to particular person Issue is used.Different labels are also used to clarify more about an issue.You can collect user feedback, report software bugs, and organize tasks you'd like to accomplish with issues in a repository.

**Steps to create issues:**
1.Go to the repository page in which you want to create issue.
2.Click on issues.
3.Click on create new issue.
4.Type issue in comment box you can add labels like bug,enhancement,etc.
5.Submit the issue. 
