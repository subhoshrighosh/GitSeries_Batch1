# About Git
Git is a free and open source distributed version control(Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.
For example:If you are a graphic or web designer and want to keep every version of an image or layout which you would most certainly want to, a Version Control System (VCS) is a very wise thing to use) system designed to handle everything from small to very large projects with speed and efficiency. 

Git is easy to learn and has a tiny footprint with lightning fast performance.
It was created by Linus Torvalds in 2005 for development of the Linux kernel, with other kernel developers contributing to its initial development.

It is designed for coordinating work among programmers, but it can be used to track changes in any set of files.
Its goals include speed, data integrity, and support for distributed, non-linear workflows.
Git supports rapid branching and merging, and includes specific tools for visualizing and navigating a non-linear development history. 
In Git, a core assumption is that a change will be merged more often than it is written, as it is passed around to various reviewers. 
In Git, branches are very lightweight: a branch is only a reference to one commit. With its parental commits, the full branch structure can be constructed.

## Git setup:

### Your Identity

The first thing you should do when you install Git is to set your user name and email address. This is important because every Git commit uses this information, and it’s immutably baked into the commits you start creating:

$ git config --global user.name

$ git config --global user.email

### Your Editor

Now that your identity is set up, you can configure the default text editor that will be used when Git needs you to type in a message. If not configured, Git uses your system’s default editor.

# About GitHub

GitHub is the single largest host for Git repositories, and is the central point of collaboration for millions of developers and projects. 
A large percentage of all Git repositories are hosted on GitHub, and many open-source projects use it for Git hosting, issue tracking, code review, and other things.
It provides cloud storage for source code, supports all popular programming languages, and streamlines the iteration process.

## Git workflow:

The idea is simple: 
•There is one central repository. 
•Each developer clones the repo, works locally on the code, makes a commit with changes, and push it to the central repository for other developers to pull and use in their work.

## Different stages of git Project:

### Modified-
Initializing a Repository in an Existing Directory using Command:
$ git init
This creates a new subdirectory named .git that contains all of your necessary repository files 

Cloning an Existing Repository:
If you want to get a copy of an existing Git repository, the command you need is 
$git clone <url>

Checking the Status of Your Files:
The main tool you use to determine which files are in which state is the git status command. 
Run this command directly after a clone, you should see something like this:
$ git status

On branch master
Your branch is up-to-date with 'origin/master'.
nothing to commit, working directory clean.

### Staged-

Tracking New Files-
In order to begin tracking a new file, you use the command git add. To begin tracking the README file, you can run this:
$ git add README
So, we saw that we can make changes to the project.We use the commands in the Git command line — git add.This command tracks the new changes and pushes it to the staging area. 
So, staging area is place prior to the actual implementation of changes, i.e. this area contains all the added files that contain new code, which are ready to be joined to the remote repository. 
Therefore,all the new files are first pushed to the staging area.

### Commit-
This is the final stage, as this stage finally applies the new changes to the remote repository. So, a commit is a set of new files that are being added to a project as part of the modification. Each commit represents the changes made to project in the past, with the details about the time at which commit was made and the author of the code. 

The simplest way to commit is to type $ git commit
So, finally when you make a commit, and it gets committed, then this simply means that you have successfully applied a certain modification to the code.

## Git Branching:
A branch is a lightweight movable pointer to one of these commits. The default branch name in Git is master . As you start making commits, you're given a master branch that points to the last commit you made. Every time you commit, the master branch pointer moves forward automatically. 

### Creating a new Branch:
The $ git branch command lets you create, list, rename branches.

### Switching Branches:
To switch to an existing branch, you run the git checkout command.

### To delete branch:
Use Command $ git branch -d.
The -d option will delete the branch only if it has already been pushed and merged with the remote branch. Use -D instead if you want to force the branch to be deleted, even if it hasn't been pushed or merged yet.

## Basic Merging-
It is a process of merging a new branch into master branch.

### Creating Merge Conflict-
This code example executes a sequence of commands that accomplish the following.

•Create a new directory named git-merge-test, change to that directory, and initialize it as a new Git repo.

•Create a new text file merge.txt with some content in it.  

•Add merge.txt to the repo and commit it.
Now, we have a new repo with one branch master and a file merge.txt with content in it. 

•Next, we will create a new branch to use as the conflicting merge.

•Create and check out a new branch named new_branch_to_merge_later

•Overwrite the content in merge.txt 

•Commit the new content

•git merge new_branch_to_merge_later

A conflict appears

### To resolve Conflict-
•The most direct way to resolve a merge conflict is to edit the conflicted file. 

•Open the merge.txt file in your favorite editor. 
For our example lets simply remove all the conflict dividers. 
Once the file has been edited use git add merge.txt to stage the new merged content. 

To finalize the merge create a new commit
Git will see that the conflict has been resolved and creates a new merge commit to finalize the merge.

# Making a Pull Request:
Pull requests are a feature that makes it easier for developers to collaborate using Bitbucket. They provide a user-friendly web interface for discussing proposed changes before integrating them into the official project.

When you file a pull request, all you’re doing is requesting that another developer (e.g., the project maintainer) pulls a branch from your repository into their repository. This means that you need to provide 4 pieces of information to file a pull request: the source repository, the source branch, the destination repository, and the destination branch.

Using pull requests with each of these workflows is slightly different, but the general process is as follows:
1)A developer creates the feature in a dedicated branch in their local repo.
2)The developer pushes the branch to a public Bitbucket repository.
3)The developer files a pull request via Bitbucket.
4)The rest of the team reviews the code, discusses it, and alters it.
5)The project maintainer merges the feature into the official repository and closes the pull request. 

# Creating an Issue:
Issues can be used to keep track of bugs, enhancements, or other requests.
Any GitHub user can create an issue in a public repository where issues have not been disabled.
1)You can open a new issue based on code from an existing pull request.
2)You can open a new issue directly from a comment in an issue or a pull request review.

## Steps for creating an issue-
1)On GitHub, navigate to the main page of the repository.
2)Under your repository name, click Issues. 
3)Click New issue. 
4)If there are multiple issue types, click Get started next to the type of issue you'd like to open. 
5)Type a title and description for your issue. 
6)If you're a project maintainer, you can assign the issue to someone, add it to a project board, associate it with a milestone, or apply a label.
7)When you're finished, click Submit new issue.

#### This was all about Git and working of GitHub.





