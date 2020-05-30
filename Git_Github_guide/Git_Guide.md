# Introduction to Git and Github

## Git
Git is a version control system that is widely used in the programming world. It is used for tracking changes in the source code during software development. It was developed in 2005 by Linus Torvalds, the creator of the Linux operating system kernel.

### Github
Projects on GitHub can be accessed and manipulated using the standard Git command-line interface and all of the standard Git commands work with it. GitHub also allows registered and unregistered users to browse public repositories on the site. Multiple desktop clients and Git plugins have also been created by GitHub and other third parties that integrate with the platform.


# Formats and features supported by Github

In addition to hosting source code, GitHub supports the following formats and features:
 
+ **Documentation**, including automatically rendered README files in a variety of Markdown-like file formats (see README files on GitHub)
+ **Issue tracking** (including feature requests) with labels, milestones, assignees  and a search engine
 
+ **Pull requests** with code review and comments
+ **GitHub Actions**, which allows building continuous integration and continuous
  deployment pipelines for testing, releasing and deploying software without the  use of third-party websites/platforms
+ **Commits history**
+ **Graphs**: pulse, contributors, commits, code frequency, punch card, network, 
  members
+ **Integrations Directory** to name a few.


## Working of Github
The Git workflow consists of four fundamental elements.

+ Workspace
+ Index
+ Local Repository
+ Remote Repository

# Forking

A fork is a copy of a repository that allows you to freely experiment with changes without affecting the original project. A forked repository differs from a clone in that a connection exists between your fork and the original repository itself. In this way, your fork acts as a bridge between the original repository and your personal copy    where you can contribute back to the original project using Pull Requests.

**Steps to fork a Repo**

- Go to the Repo which you want to fork.
- click on fork button.

# Cloning

When you create a new repository on GitHub, it exists as a remote 3 location where your project is stored. You can clone your repository to create a local copy on your 
computer so that you can sync between both the local and remote locations of the project.
To clone a repository, head over to the main page of a project and click the Clone or download button to get the the repository’s HTTPS or SSH URL. Then, you can perform   the clone using the git clone command in your command line interface of choice. For a step by step guide, check out the cloning a repository.

**Steps to perform cloning**

+ Click on the *clone and download* button on the repo you want to clone.
+ Copy the link and open git bash.
+ Use command *git clone* and paste the link.

# Pull Requests

Many source code management tools such as Bitbucket enhance core Git functionality with pull requests. A pull request is a way to ask another developer to merge one of your branches into their repository. This not only makes it easier for project leads to keep track of changes, but also lets developers initiate discussions around their work  before integrating it with the rest of the codebase.

# What is an issue?

Issues are a great way to keep track of tasks, enhancements, and bugs for your projects. They’re kind of like email—except they can be shared and discussed with the rest of your team.One can collect user feedback, report software bugs, and organize tasks you'd like to accomplish with issues in a repository.

**Steps to create issues**

- Open the repository page in which you want to create issue.
- Click on the issues button.
- A new window opens ,click on create new issue.
- Type the issue in comment box add labels like enhancement,bug etc.
- Submit the issue. 

# Merge Conflict

Merging and conflicts are a common part of the Git experience. Conflicts in other version control tools like SVN can be costly and time-consuming. Git makes merging super 
easy. Most of the time, Git will figure out how to automatically integrate new changes.
Conflicts generally arise when two people have changed the same lines in a file, or if one developer deleted a file while another developer was modifying it.

# Some commands used in github

- **git status**
  Usage: git status  
  This command lists all the files that have to be committed.

- **git commit**
  Usage: git commit -m “[ Type in the commit message]”
  This command records or snapshots the file permanently in the version history.

- **git clone**
  Usage: git clone [url]  
  This command is used to obtain a repository from an existing URL.

- **git add**
  Usage: git add [file]  
  This command adds a file to the staging area.

- **git pull**
  Usage: git pull [Repository Link]  
  This command fetches and merges changes on the remote server to your working directory.
- **git config** 
  Usage: git config –global user.name “[name]”  
  Usage: git config –global user.email “[email address]” 
 
- **git branch**
  Usage: git branch  
  This command lists all the local branches in the current repository.

 - **git checkout**
   Usage: git checkout [branch name]  
   This command is used to switch from one branch to another.
 
- **git push**
  Usage: git push [variable name] master  
  This command sends the committed changes of master branch to your remote repository.



regards 
Pragya Diwakar
