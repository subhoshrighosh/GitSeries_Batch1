## Everything about GitHub!!

*Hello! This document will contain everything about Github, its working and its features.<br>*

*Git is a distributed version control tool and helps in merging different source code. From version control system I mean that it helps in recording and managing a project's source code and its past versions as well. It helps in keeping track of changes made in a source code and all this is done with the help of repositories  which it maintains and managing them. It is a open source tool and is completely self sufficient, installed on our local system rather than in the cloud.<br>*

*Github is a cloud-based hosting service used to host open source projects and thus help in bringing team together. It is used to manage Git-repositories.<br>

*Github is so popular in most of the projects because:
(A) It provides secure cloud storage for source code<br>
(B) It has collaboration feature which helps in bringing team together.<br>
(C)It supports all programming languages.<br>
(D)It came up with a Model-view-presenter.<br>*

### WHAT IS GITBASH?

*Git Bash is an application for Microsoft Windows environments which provides an emulation layer for a Git command line experience. Bash is an acronym for Bourne Again Shell. A shell is a terminal application used to interface with an operating system through written commands.<br>*


### Git Overflow

*There is one Central repository. Any developer who wants to make any changes clone that repository and make changes locally using commit command. Then pushes it to the central repository so that any other developer wanting to make any change can pull and use in their work.<br>*

#### Different stages of a Git Project

Git Workflow consist of the four fundamental elements: <br>
•  **Workspace**(also known as Working Directory) and if we consider a file, it can have 3 states:
 (a)Committed : meaning latest changes in the data is stored in local repo.<br>
 (b)Modified: means the changes are done but are not securely stored or will not be reflected in local repository.<br>
 (c)Staged: meaning file is part of index element.<br>

• **Index**(also known as Stage)<br>
• **Local Repository**(also known as Head)<br>
• **Remote Repository**<br>
  
**CLONE COMMAND**: If we are gaining access to a remote repository then we need to clone it by following it by URL using git clone command which will create a local cpopy of repository in our workspace.<br>

**ADD COMMAND**: This command will add the file in the workspace in the index stage and thus we call this file as staged file.<br>

**COMMIT COMMAND**:  This command will commit all files that are staged with their changes and are safely stored.<br>
               We can perform these add and commit commands in a single defined command as commit -a which helps in commiting all files at once if they are part of repository and already known.<br>

**PUSH COMMAND**: It pushes the changes that are in the local repository to the remote repository and anyonce having access to this remote repo can see the changes.<br>
 
For opposite flow we have following commands:

**FETCH COMMAND**: Used to get files from the remote repository to local repository.<br>
**MERGE CAMMAND**: It get changes from local repo and get them to workspace.<br>
**DIFF COMMAND**: Used to tell the difference between files which are in workspace and ones which are stagged for commit.<br>

### Initializing a Git repo

(a) Go to the account and click option NEW repository.<br>
(b) We can give a repository name and make a README file<br>
(c) Then in gitbash, enter the repository by writing **cd repo_name**.<br>
(d) Then for initializing this repository, use command : **git init**.<br>
(e) Make a file inside this repo and add this your repo using **git add . command**.<br>
(f) Then for commiting it use command : **git command -m "Message here"**.<br>
(g) Then push it to the repository using command : **git push -u repo_name master**.<br>


### Fork and Clone in Git

*Fork in git means making a personal copy of someone else's project or repository which helps us to modify and make changes in it without affecting the orignal project. It acts as a bridge between orignal repo and the copy we made.<br>
*Clone is used to create  a local copy of the remote repository.This process helps us to edit and modify files locally.<br>*

We can fork any repository by clicking the fork option on the right side of the repository.<br>

For cloning the repository, we need to use command line and provide the following command:<br>
(a) First go the repository <br>
(b) Then click clone or download option under repository.<br>
(c) Copy the URL name.<br>
(d) use command git clone URL<br>

### Branches in Git

*A branch in github can be said as individual project or files inside a git repository. These files are not a part of main default branch of a git repository known as "master branch" which keeps the default commits we make.<br>*
*For making a link of these projects, we can merge this branch to the master branch.<br>*
*Master branch is the default master branch of a project.<br>*
*We can have as many branches as we want and can also delete master branch by making any other branch as default one.*

#### Making a new branch:

Use command :
**git branch branch_name**

To enter into a branch use command :
**git checkout branchname**

To see list of all branches in your project use command :
**git branch -ls**

To delete a branch, use command :
**git branch -d branch_name**

### What are Pull requests??

*PR, Pull Request can be seen as informing others about the changes you have made in a particular project of a particular branch.
*Once we make a pull request, we are requesting other developer to review the changes we have made and if approved, they can merge our project into the master branch.<br>*

#### How to make a Pull Request(PR)??

(a)Clone a repository<br>
(b) Enter the cloned repository from your account.<br>
(c) Make a directory using command **mkdir**.<br>
(d)Enter the directory using command cd directory_name.<br>
(e)Add some text files in this directory by either physically going to it in your system or by command : **echo "Content" > fileName.txt**<br>
(f)Now using command : **git add fileNme.txt** , add the file.<br>
(g)Commit the file: **git commit -m "Message"** <br>
(h)Now push it to the repository using command : **git push origin master**.<br>
  Here if we are doing this by making any other branch, We need to push it by first usng git pull command and then by using **git push --set-upstream origin branch_name.**<br>
(i)Now go the repository and click Create pull request option.<br>
(j)Provide a good name for PR and a good description as well, and then Click option Compare and then see the base and head repository.<br>
(k)Click create pull request and your PR will be opened until and unless the head of the repository merges it.<br>


### Merge Conflicts

*In Git, "merging" is the process of combining another branch into our current working branch. We are taking changes from another context  and combining them with  current working files.<br>*
*However, there are some situations where we might have tell Git what to do while merging. This is when changing the same file. In this case, if two people changed the same lines in that same file, or if one person decided to delete it while the other person decided to modify it, Git simply cannot know what is correct. Git will then mark the file as having a conflict <br>*
*This is known as merge conflict.<br>*
*A merge conflict is an event that occurs when Git is unable to automatically resolve differences in code between two commits.*
*Merge conflicts can happen when merging a branch, rebasing a branch, or cherry picking a commit.<br>*

#### Creating a merge conflict

(a)Either make a git repository or enter into your git repository using cd command and initialize it using : **git init.**<br>
(b)Now make a text file names merge.txt and add content to it.
  **echo "Content" >> merge.txt**<br>
(c)Add this by using **git add merge.txt**<br>
(d)Commit it by using **git commit -am "Message"**<br>
(e)Now, one file name with content is made in the repository.<br>
(f)Now make a new branch and enter into it using command " **git checkout -b newbranch.**<br>
(g)Override the content in merge.txt file using command : **echo "Content_2" >> merge.txt**<br>
(h)Now commit it using : **git commit -am "Message"**<br>
(i)Now enter your master branch using : **git checkout master**<br>
(j)Now write **echo "Content to append" >> merge.txt**<br>
(k)commit it<br>
(l)Now write :  **git merge newbranch.**<br>


*WE will see a conflict occuring. This is called a merge conflict when we are trtying to change content of the file in same line together and trying to commit.<br>*

### Viewing the merge conflict

(a)Use command : **git status** to see the merge conflict.<br>
(b)The  use **cat merge.txt** to see the conflict and its cause.<br>

*We see many wierd signs like <<<<<<<, >>>>>>> and ========.*
*These are called conflict dividers and we need to erase them to solve the merge conflict.<br>*

### Solving a merge conflict

(a) To solve the merge conflict, we need to open the text file called merge.txt.<br>
(b) After entering the file, we need to delete all the conflict dividers<br>
(c) After deleting it, save the file and write command: **git commit** and then push it.<br>

Merge conflict is solved.<br>

### Issues in Git

Use issues to track ideas, enhancements, tasks, or bugs for work on GitHub Enterprise. You can collect user feedback, report software bugs, and organize tasks you'd like to accomplish with issues in a repository. Issues can act as more than just a place to report software bugs.<br>

### Creating an Issue in Git:

(a)To create an issue, clone a repository or make it in your own repository.<br>
(b)Go to the option issue.<br>
(c)Give a good name to your issue and a good description to it.<br>
(d)We can add labels to it by which we can tell which kind of issue it is like bug label etc.<br>
(e) We can also make our own label.<br>
(f)Then click Create issue and your issue is created/opened.<br><br>
(g)We can add comments to it and can resolve it.<br>



**This was a small guide to GitHub, its use and working.**






