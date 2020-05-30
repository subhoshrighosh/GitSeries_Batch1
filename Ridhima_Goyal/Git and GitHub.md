## Git and GitHub

Git is a distributed version control tool that can manage a development project's source code.
Git is an Open Source Distributed Version Control System.
Git also tracks the history of changes to a project’s source code including what specifically has been changed and who has 
changed what parts and when have they been changed, this feature is termed as Version Control.

GITHUB:-

GitHub is a open source platform built around the Git tool.
It allows developers to host their files in a Repository, so that others can collaborate and make suggestions on projects.
A GitHub repository can be used to store a development project. Git is a distributed version control tool that can manage 
a development project's source code.

It provides cloud storage for source code, supports all popular programming languages, 
and streamlines the iteration process.
It provides us with separate public and private repositories and easy version control.

Some other platforms similar to GitHub are:-
1) GitLab
2)BitBucket
3)Source Forge

----------------------------------------------------------------------------------------------------------------------------------------
## Git WorkFlow

The developers clones the central repository.
The edits which are made to the files by using commit command are stored locally and the pushed to the central repository.

Different stages :-

Modified:
      In a repository you can maintain and write a code. When any modification are made then it can only be 
      done on the remote repository, that simply means changes in the code can be done without changing the original code.
Staged:
      It comes before the actual implementation of changes.The new files are pushed to the staging area and 
      then joined to the remote repository.
Commit:
      Commit is a set of new files added to the project as a part of modification to the remote repository.
-----------------------------------------------------------------------------------------------------------------------------------------
## Making the first repository 

Step 1: Install Git and create a GitHub account
Step 2: Create a local git repository 

		To initialize a git repository in the root of the folder, run the "git init" command

Step 3: Add a new file to the repo

		After creating the new file, you can use the "git status" command to see which files git knows exist.
		
Step 4: Add a file to the staging environment

		Add a file to the staging environment using the "git add ." command.   

Step 5: Create a commit
	
		Run the command git commit -m "Your message about the commit"

Step 6: Create a new branch

	 	Run git checkout -b <my branch name>. 

Step 7: Push a branch to GitHub
	
		 Run git push origin yourbranchname.
------------------------------------------------------------------------------------------------------------------------------------------
## Forking and Cloning

Fork in git means making a personal copy of others repository which we can modify
without affecting the orignal project.

Clone is used to create  a local copy of the remote repository.This process helps us to edit and modify files locally.

## Cloning a Git Repo without Fork

Step 1: Clone a Repository: The user starts from the upstream repository on GitHub. Since the user navigated to the repository because he/she is interested in the concept and they like to contribute. This process starts from cloning when they clone the repository it into their local machine. Now they have the exact copy of the project files on their system to make the changes.

Step 2: Make the desired changes: After cloning, contributors provide their contribution to the repository. Contribution in the form of editing the source files resulting in either a bug fix or adding functionality or maybe optimizing the code. In this step, a contributor can apply a single commit or multiple commits to the repository. But the bottom line is, everything happens on their local system.

Step 3: Pushing the Changes: Once the changes or commits are done and now the modifications can be pushed to the upstream repository. 

## Cloning a Git Repo after Forking

Step 1: Fork a Repository

Step 2: Clone a Repository

Step 3: Make the desired changes

Step 4: Pushing the Changes

Step 5: Send changes to Original Repository: This process is called Pull Request in Git. At this step, the user sends the changes to the owner of the repository as a 
request to merge the changes to the main central repository. 
-----------------------------------------------------------------------------------------------------------------------------------------
## Branches in Github

A Git Branch is a separate line of development in a software project. 
User can create a branch, and keep on committing their changes to this branch without messing the original 'master' branch.

Usually, each developer working on a code makes his/her changes in a separate branch.
Git offers features to merge the branch with the master branch after changes are done. 
The branches can also be named according to what kind of changes they contain. 
-----------------------------------------------------------------------------------------------------------------------------------------
## Pull Request(PR)

A pull request is submitted when you’ve worked on some code from a particular branch and want to inform 
the others of the changes you’ve made. people can be assigned to review and subsequently approve the request 
before your changes can be incorporated into the branch.

Sometimes you'll be a co-owner or the sole owner of a repo, in which case you may not need to create a PR to merge your changes.
However, it's still a good idea to make one so you can keep a more complete history of your updates and to make sure you always create a new branch when making changes.
-----------------------------------------------------------------------------------------------------------------------------------------
## Merge Conflict

Conflicts arise when two people have changed the same lines in a file, 
or if one person deleted a file while another person was modifying it. 
In these cases, Git cannot automatically determine what is correct. 
Git will mark the file as being conflicted and halt the merging process. 
Resolving the merge conflict in GitHub:-

Step 1: git branch
Step 2: git checkout master
Step 3: git merge yourbranchname
 


