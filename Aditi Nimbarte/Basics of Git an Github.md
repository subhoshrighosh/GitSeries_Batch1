# Introduction to Git and Github

### **Git**
    -Git is an Open Source Distributed Version Control System.It is a command line tool. Git can be used to store content,it is mostly used to store code due to the other features it provides.Version Control System helps in handling this by maintaining a history of what changes have happened. Also, Git provides features like branches and merges.Multiple developers can work parallely with no code conflicts. It uses repositories to store the changes made in source code. 

### **Github**
	-GitHub is a Git repository hosting service, but it adds many of its own features.GitHub provides a Web-based graphical interface. It also provides access control and several collaboration features.GitHub makes it easy to share code between multiple computers and developers.

**Github is popular due to following reasons**
1. It provides cloud storage for source code, supports all popular programming languages
2. Easy version control.
3. Secure Cloud Storage.
4. Teams can work together easily.

**Git works on four fundamental elements**
1. Workspace-working directory
2. Index(stage)-project is added and ready to be commited
3. Local Repository-it resides in our systems and contains all the files with their commit history
4. Remote Repository-repository on the server to which every member will have access

**Different stages of Git project:**
1. Modified: We can make changes to copy of our project without hampering the orignal code.
2. Staged-the files which are added and ready to be commited but not yet commited. 
3. Commit-the staged files are commited to local repository.

### Git Commands


**git init** -  This command adds a local Git repository to the project.

**git add .** -it adds all the files and folders in your project to the staging area.

**git add *filename*** - it adds the specific file in staging area.

**git commit -m "<*enter the message about commit*>"**- Records changes to the repository.

**git status**-This command will give you a list of all the updated, added and deleted files.

**git branch**- It will show master branch with *

**git checkout** -It will how the branch we are currently working on.

**git pull**-to pull the latest changes from the remote repository into the local repository.

**git log**- to print out all the commits which have been done up until now.  

**git push**- to push all the code from the local repository into the remote repository.

**git clone *url***-to clone an existing remote repository into your computer.url of remote repository.

**git merge *branch name***- it wil merge currently working branch with the branch.

### Github 

**Fork** : A fork is a copy of a repository that you manage. Forks let you make changes to a project without affecting the original repository. You can fetch updates from or submit changes to the original repository with pull requests.

**Pull Request(PR)**: Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch.

**Issues** :Issues can be used to keep track of bugs, enhancements,Merge conflicts or other requests.

**Labels** :Labels on GitHub help you organize and prioritize your work.
 
**Merge Conflicts**:Git can handle most merges on its own with automatic merging features. A conflict arises when two separate branches have made edits to the same line in a file, or when a file has been deleted in one branch but edited in the other. Conflicts will most likely happen when working in a team environment.

*Before starting project you need to have an github account and set git username*
### How to initialize project -
- To begin, open git bash and move to where you want to place the projec-t on your - local machine using the cd (change directory) command. 
- To initialize a git repository in the root of the folder, run the *git init* command.
Go ahead and add a new file to the project, using any text editor 
- Add a file to the repository in staging environment using the *git add .* command.
- Run the command *git commit -m "Your message about the commit"*
- then push it using *git push origin repo_name*

### How to fork and clone project -
- Login to your github account open the repository in which you want to contribute
- then click on the *fork* option,present on the upper right hand side of the page
- you will be redirected to the fork repository,then click on *clone or download* copy the *url*.
- now in you terminal type *git clone url*
- project is cloned now you can modifiy it.

### Creating a new branch
- to create a new branch use command *git branch branch_name*
- to enter into the branch use command *git checkout branch_name*
- to delete branch use command *git branch -d branch_name*
- to view all branches type *git branch -ls*

### Creating a Pull Request
 After modifing the project if you want to merge it with the orignal then you need to make request to the owner
 - In your forked repository there is option *pull request* click on it.
 - it will redirect you to the compairing page,here you need to select *base repository* the orignal repository and the *head repository* which is modified version of orignal repository*
 - now,click on compare 
 - make sure you have assigned good name to your pull request and good description.

 
### Resolving merge conflicts
- create two new branches by using command *git branch branch1* and *git branch branch1*
- edit the same file written in markdown language and write different content 
- then use command *git checkout branch1*
- and now, merge branch2 with branch1 using *git merge branch2* 
e.g:- I created a merge conflict using git bash where I created a temp branch and added new line to my introduction saying "i like c language for programming" ,then i created another branch named temp2 where i write "i like python language for programming". After that, I merged the temp1 branch with the temp2 branch it showed merge conflict because it get confused which statement is true 
- then use command *git cat filename*
We will see the seperators <<<<<< ,===== and  >>>>>>
we have to remove them in order to solve conflict
- we can remove the statement above === or below it depending on reliability
- add this changes to repo, commit them and push it to the remote repository.
- now you can merge the branches.

### Creating Issues on Github-
- Open the repository go to the option *issue
- write a name of issue and give a proper description 
- we can use default labels or create the label.
- we can add images/screenshot to the issue by just a drag or else using url.
- Click on create issue,issue is created.

***Thank you for reading,hope it's helpful.***



