# ***Git and Github Basics***

## ***Git***
**Git** is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
Git is created by *LINUS  TORVALDS*. It is an open-source, free, and *distributed version control system*. Git has trunk-based development in it which involves branches in the repository in which we can create a new branch even while working with the current branch and also we can merge the new branch with the master branch if required at any point.

## ***Github***
**Github** is a website in which we can upload projects that have version control over them. GitHub is a file or code-sharing service to collaborate with different people. GitHub, which is delivered through a software-as-a-service (SaaS) business model, was started in **2008** and was founded on Git, an open source code management system created by ***Linus Torvalds*** to make software builds faster.
**Other Platforms similar to Github are:**
*a. GitLab
 b. BitBucket
 c. Source Forge
 d. AWS Code Commit*
 
**GitHub is popular as:**
*• Largest shared repository
 • Separate public and private repositories
 • Shared Repositories which can be accessed by millions of users and make contributions to existing files or codes
 • Easy Version Control
 • Can be accessed anytime and anywhere*


## ***Github Workflow***
There is one central repository. Each developer clones the repository, works locally on the code, makes a commit with changes, and push it to the central repository for other developers to pull and use in their work.
a). **Workspace:**
The *Workspace* is the area where we are currently working. It is where our files are stored. If we make changes to files in your workspace git will recognize that they are modified.To know what is stored in our file: Run the command git status. This command will show you two things: The files in your Workspace and the files in your Staging Area. 

b). **Staging Area** 
The *Staging Area* is when git starts tracking and saving changes that occur in files. These saved changes reflect in the .git directory. If you want to track specific files, then git moves from Workspace to the Staging Area. If you make any more additional changes after adding a file to the Staging Area, git will not know about those specific changes until you tell it to see them. We explicitly have to tell git to notice the edits in our files. To know which files are in staging area click git status.

c). ***Local Repository***
The *Local Repository* is everything in our .git directory. Mainly what we will see in your Local Repository are all of our checkpoints or commits. It is the area that saves everything.
To add items from our Staging Area to our Local Repository: The git command git commit takes all changes in the Staging Area, wraps them together and puts them in our Local Repository. A commit is simply a checkpoint telling git to track all changes that have occurred up to this point using our last commit as a comparison. After committing, your Staging Area will be empty.

d). ***Remote Repository***
As we make changes to our project locally on our system, we can keep them up-to-date with our remote repository. In Git, a remote is the server where our code is stored. In our case, that server is a repository on GitHub.

## ***Forking***
A fork is a copy of a repository. Forking a repository allows us to freely experiment with changes without affecting the original project.

## ***Cloning***
When we clone a repository, the repository is copied to our local machine with the help of Git.

## ***Branches***
Using *branches* we can seperate our work from the main file. There is a default branch called **master branch**. To avoid mess up in the master branch we create local branches.

***Switch Branch***
We can switch from one branch to the other branch by using a command. The command is listed below:
git checkout <Branch_Name>

***Deleting Branch***
We can delete branch by using the following commands:
git branch -d <branch_name>

*Note:*We cannot delete a master branch because it get activated by default when we use the command "git init".

## ***Pull Request***
PR stands for Pull Request. This request is used to ask the person to merge our changes in his repository .We use this command after forking and clonning somone else project. When you file a pull request, all you’re doing is requesting that another developer pulls a branch from your repository into their repository. This means that you need to provide four pieces of information to file a pull request: the source repository, the source branch, the destination repository, and the destination branch.
**Making a pull request**
*1. Fork the repository of a person on which you wants to work.
2. Clone that repository.
3. Make the changes as per your requirement.
4. Add and commit the files.
5. Then perform the pull command.
6. Finally we can make a pull request to the owner from the github.*

## ***Commit***
The ***"commit"*** command is used to save your changes to the local repository. Note that you have to explicitly tell Git which changes you want to include in a commit before running the *"git commit"* command. This means that a file won't be automatically included in the next commit just because it was changed. 

## ***Merge Conflict***
*Conflicts* occurs when two person changes the same lines in a file, or one person deletes a file and another person modify it. Git is unable to  automatically determine the correct one.

**Resolving Conflict**
 *1. We can see the file and the conflicts in it using the command "cat <file name>"
  2. We can go the file in the folder on local machine and can edit as per the requirements.
  3. Finally,we need to add and commit the file.*
  
## ***Issues***
*Issues* can be used to keep track of *bugs, enhancements, or other requests*.You can collect user feedback, report software bugs, and organize tasks you'd like to accomplish with issues in a repository. Issues can act as more than just a place to report software bugs.

## ***Steps for creating Issue***
*1. To create an issue, clone a repository or make it in your own repository.
2. Go to the option issue.
3. Give a good name to your issue and a good description to it.
4. We can add labels to it by which we can tell which kind of issue it is like bug label etc.
5.  We can also make our own label.
6. Then click Create issue and your issue is created/opened.
7. We can add comments to it and can resolve it.
8. To create an issue, clone a repository or make it in your own repository.
9. Go to the option issue.
10. Give a good name to your issue and a good description to it.
11. We can add labels to it by which we can tell which kind of issue it is like bug label etc.
12. We can also make our own label.
13. Then click Create issue and your issue is created.
14. We can add comments to it and can resolve it.*



