# **GUIDE ABOUT GIT/GIT HUB**

**GIT :**

*Git is a ```distributed control version software``` i.e. it helps us to keep the record of the history in the form of remote and local repo(repository) so that we can access the history any time without any obstruction.Version control system means that it helps in  managing a project's source code. It helps in keeping track of changes made in a source code and repositories manages all the edits or changes. It is a open source tool and you can load the repositories in your local repository or in your local system as well.

**GITHUB :**

*GitHub is a ```website or web service``` which allows people to perform social coding which has version control on them i.e. Git*

* *It prevents you from messing up your own code. If you use github, you don’t have to worry too much about accidentally deleting important stuff or breaking your entire app because you accidentally deleted a semicolon.*

* *It lets others watch what you are doing to your app.*

* *You and your friends can work on the same app together, without stepping on each other’s toes. Otherwise if you both write code onto the same file, whoever saved first will lose everything they wrote because whoever saved last overwrites the file. This doesn’t happen if you use git.*

###### NOTE: One dont need to know about both, one can eaily be oriented on GIT or GITHUB,and also one can work using both GIT and GITHUB too.

*Git has a work-flow, i.e. **```add-->commit-->push-->pull```***
1. Creating branch(by default master) and then creating the files and working on it.
2. adding the file(s) and commiting the file(s).
3. Merge your other branch if you have created any with master if your newly created branch worked perfectly or else modify.
The files will be stored in local and remote repo so that we can access our project anytime.

### **COMMON COMMANDS**

* *```ls``` ---> This will list all the files in the directories.*
* *```git config``` --->  Short for “configure,” this is most useful when you’re setting up Git for the first time.*
* *```git init``` ---> Initializes a new Git repository. Until you run this command inside a repository or directory, it’s just a regular folder. Only after you input this does it accept further Git commands.*
* *```cd (name of directory)``` ---> it will take you to that directory.*
* *```cd ..``` ---> it will take you out of that directory. *
* *```mkdir (name of directory)``` ---> it will create a directory of the name you mentioned.*
* *```git status``` ---> Check the status of your repository. See which files are inside it, which changes still need to be committed, and  which branch of the repository you’re currently working on.*
* *```clear``` ---> clear the screen*
* *```cat file.txt``` ---> it shows the content present in the file.

#### **OPENING FIRST REPOSITORY/REPO :-**

1. Create a Github account, by using you e-mail account and signup

2. Create a new repository -> To create a new repository, select New Repository from the + sign dropdown menu -> Enter a name for your repository

3. download and install git from offical website if not already installed ->run gitbash.exe ->It will open a terminal in windows\mac\linux

4. ```$ mkdir NAME ->$ cd NAME ->$ echo "#NAME" >> Readme.md``` --->This will create a directory at local with name "NAME", 
whcih will have a text file "Readme.md" ->$ cat Reamde.md ->This will show the contents of the file ->To tell your computer that Demo is a directory managed by the Git program, enter: ->$ git init ->Then, to tell the Git program you care about this file and want to track any changes from this point forward, ->$ git add Readme.md

5. Making a commit ->So far you've created a file and told Git about it, and now it's time to create a commit. Commit can be thought of as a milestone. Every time you accomplish some work, you can write a Git commit to store that version of your file, so you can go back later and see what it looked like at that point in time. Whenever you make a change to your file, you create a new version of that file, different from the previous one. ```git commit -m "commit"``` --->You just created a Git commit and included a message that says first commit.

6. Connect your GitHub repo with your computer **git remote add origin (remote_url)** ---> Now we have connected our local copy of the NAME repository to its remote counterpart on GitHub. Now that we have added the remote, we can push our code to GitHub. 

**You can add more remote other than origin that which will be the topic of our discussion** 

#### **CREATING REMOTE:-**

*A remote in Git is a common repository that all team members use to exchange their changes. In most cases, such a remote repository is stored on a code hosting service like GitHub or on an internal server. In contrast to a local repository, a remote typically does not provide a file tree of the project's current state. A universal name for remote is given as **origin**, but we can name it anything according to our needs.*

*For creating remote, the command we use is :-
``` git remote add (name_of_remote) remote_url```*

*Now your remote has been created and now you can push your files in the github.
for checking the list of remote :-
```git remote``` ---> this will enlist all the remote created*

### **How it works:-**

*If you have created a file of extention say, .txt then GIT focuses or look for the changes you have made in the file. Then, it adds up the changes and reconstruct the file. It’s somewhat like human memory. It reconstructs the memory by aggregating a series of events. In Git, each of these events are called **commits**.

*But before commit, we have to create and then add the files.*

##### **CREATING FILE!**

*For creating file, you have command to create a file, i.e. **touch command**. You have to use this as follows:-
```touch file.txt``` ----> This will create a text file and not only text, you can create and multiple files of different extentions. 

##### **ADDING FILE!**

*Now for adding a file, we have **git add** command, as this will keep the files in staging mode (staging mode is the mode where you dont save the changes but add them so that u may save them later). The code is used as follows:-
```git add file.txt``` ----> Now the file.txt is added successfully!.

*You may add multiple files at once using ``` git add .``` command, it will add all the files at once.*

##### **COMMITING THE FILE!**

*Now for commit, Everything is a collection of commits. However, just saving a file won’t automatically turn it into a commit.
You need to tell git that this change (or a set of changes) is a commit. You do this by running the command called commit. Then you add a message next to it:-* 

``` git commit -a``` ----> This command means that you want to all the files which you add

```git commit -m "i am commiting the change"``` ----> This means you want to commit while passing a message

```git commit -am"i am commiting the change"``` ----> This means you want to commit all the changes with a message.

##### **PUSHING YOU FILES TO GITHUB**

*The git push command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo. It's the counterpart to git fetch , but whereas fetching imports commits to local branches, pushing exports commits to remote branches.*

*We use the following commands :-
```git push (name_of_remote) master``` ---> This means, the files which has been commited will be pushed to github via remote in the **branch - master**.

##### **BRANCHES IN GIT/GITHUB**

*A branch in Git is simply a lightweight movable pointer to one of these commits. The default branch name in Git is **master**. As you initially make commits, you're given a master branch that points to the last commit you made. Every time you commit, it moves forward automatically.*

*To create Branches, we use the following commands:-*

* *```git branch (name_of_new_branch)``` ---> creates new branch*
* *```git checkout (name_of_new_branch)``` ---> moves you from master to the other branch*
* *```git checkout -b (name_of_new_branch)``` ---> this will let you create a new branch also switch you to the respective branch.*

*If you want to check the list of the branches, you can use ```git branch``` command as it will enlist you the branches you have created as of now.

#### **MERGING BRANCHES**

First we run ```git checkout master``` to change the active branch back to master. Then we run the command ```git merge new-branch``` to merge the new feature into the **master branch**. 
**Note that git merge merges the specified branch into the currently active branch. So we need to be on the branch that we are merging into.**

#### **FORKING**

*A fork is a copy of a repository that allows you to freely experiment with changes without affecting the original project. A forked repository differs from a clone in that a connection exists between your fork and the original repository itself. In this way, your fork acts as a bridge between the original repository and your personal copy where you can contribute back to the original project using Pull Requests.*

*Steps for forking a repository:-
> Go to repository, that you want to fork. 
> On top right corner you will se a button **'Fork'**, click that button.
> It will tell you to wait for seconds and thus forking repository will happen.*

#### **CLONING**

*Git clone is primarily used to point to an existing repo and make a clone or copy of that repo at in a new directory, at another location. The original repository can be located on the local filesystem or on remote machine accessible supported protocols. The git clone command copies an existing Git repository.*

*Steps for cloning:-
> Go the the repo who you want to clone the repo(repository)
> Copy the URL of the repo.
> Open up the GITBASH, and use the command:-
```git clone (paste the url copied)``` 
>GIT will process and create the clone of the repo to your local system.

#### **PR : PULL REQUEST**

*Pull Request allows others to know about the changes one has pushed in the github repository.
A Pull Request is submitted when you’ve worked on some code from a particular branch and want to inform the others of the changes you have made. So after forking a project we can pull request.*

**Steps for creating PR:-**

* After forking and cloning the project or file to your local system, open your Git.

* Make the changes you want to in the cloned file uing git commands.

* After modifying, add, commit and push it on github.

* Enter your username and password to the prompt window.

* On github, Click on **```"Compare and Pull Request button"```**.

* Click on **```Create pull request```** to open a new pull request. Enter the title and desctription of the pull request and send the request.

## **MERGE CONFLICTS:-**

*When we merge the branches, if in the file, more than one person has commited change in the perticular line of the file with different set of data and send pr (pull request) to the remote repo, this act will creates a **merge conflict**.   

### *CREATING MERGE CONFLICTS:-*

*Steps taken to create a **merge conflict** :-*

![merge conflict](https://user-images.githubusercontent.com/54271833/82997921-a5412c00-a024-11ea-8748-9bb78a695157.jpg)

*I created directory of my name and then file using ```touch``` command i.e. merge.txt. Then wrote the content ```(using ECHO command)```, added the file and commited it.* 

*After that created a branch named new_branch, and there i entered the content in the same file.*

*Then i switched back to master branch and entered or appended the data and finally tried for merging the branch task4 using ```git merge new_branch command```,*

*But **MERGE CONFLICT** popped up!!!* 

### *RESOLVING MERGE CONFLICTS:-*

![resolved](https://user-images.githubusercontent.com/54271833/82999650-f4885c00-a026-11ea-83fe-d30ca3561495.jpg)

*Steps taken to resolve a **merge conflict** :-*

*Once Conflict is popped up, now its essential for you to work on resolving the issue or conflict.
You can use ```git status``` command to have brief information about the conflict and your file.*

*So at first use command ```cat <filename.extenion>``` to check where the **conflict dividers** are.*

*Now your next step is to open the file i.e. merge.txt in the windows (editor) and remove all the conflict dividers and save that file. After that add and commit your file,* 

*Hence your merge conflict is **Resolved!***   



> **HOPE THIS DATA WILL HELP YOU UNDERSTAND ABOUT GIT/GITHUB**
> **THANKYOU!**
  








