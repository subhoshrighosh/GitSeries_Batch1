## Step by step guide towards github

## What is Github!!
GitHub is a highly used software which is typically used for version control. It is helpful when more than just one person is working on a project. Say for example, a software developer team wants to build a website and everyone has to update their codes simultaneously while working on the project. In this case, Github helps them to build a centralized repository where everyone can upload, edit and manage the code files. Github has many advantages over other cloub based sites like dropbox. Github document the changes and reflect them in an organized manner to avoid any chaos between any of the files uploaded.

## How Github Works!!
GitHub is a Git repository hosting service, which provides a web-based graphical interface. It helps every team member to work together on the project from anywhere and makes it possible for them to work collaboratively.
It is used widely by software developers as it allows them to store source codes for a project and track the complete history of all changes to that code. There are millions of repositories on GitHub and each repository has its own tools to help you host and release code.
GitHub helps all the team members to stay on the same page and stay organized. Moderation tools like issue and pull request locking help the team to focus on the code. GitHub is one place where project managers and developers coordinate, monitor, and update their work so projects stay transparent and on time.
Pull requests help the teams to review, improve, and propose new codes on GitHub. The implementations and proposals can be discussed before changing the source code.
The packages can be published privately, or within the team or publicly for the open-source community. The packages can be used or reused by downloading it from the GitHub.
GitHub uses tools to identify and analyze vulnerabilities to the code, that other tools tend to miss. Development teams everywhere work together to secure the software supply chain, from fork to finish.

                                    ## Guide to open your first repository

**Step 1**
->Create a Github account, by using you e-mail account and signup

**Step 2**
-->Create a new repository
-> To create a new repository, select New Repository from the + sign dropdown menu
-> Enter a name for your repository 

**Step 3**
->download and install git from offical website if not already installed
->run gitbash.exe
->It will open a terminal in windows\mac\linux

**Step 4**
[statement followed by $ will be considerd as a command to be written in terminal]
# ->$ mkdir NAME
# ->$ cd NAME
# ->$ echo "#NAME" >> Readme.md
# ->This will create a directory at local with name "NAME", whcih will have a text file "Readme.md"
# ->$ cat Reamde.md
# ->This will show the contents of the file
# ->To tell your computer that Demo is a directory managed by the Git program, enter:
# ->$ git init
# ->Then, to tell the Git program you care about this file and want to track any changes from this point forward,
# ->$ git add Readme.md

**Step 5**
-->Making a commit
->So far you've created a file and told Git about it, and now it's time to create a commit. Commit can be thought of as a milestone. Every time you accomplish some work, you can write a Git commit to store that version of your file, so you can go back later and see what it looked like at that point in time. Whenever you make a change to your file, you create a new version of that file, different from the previous one.
# ->$ git commit -m "This is a demo commit"
->You just created a Git commit and included a message that says first commit. 

**Step 6**
--> Connect your GitHub repo with your computer
# ->$ git remote add origin https://github.com/<your_username>/NAME.git
-> Now we have connected our local copy of the NAME repository to its remote counterpart on GitHub.com
->Now that we have added the remote, we can push our code (i.e., upload our README.md file) to GitHub.com

                                    **GREAT WE HAVE PUSHED OUR FIRST REPOISTORY TO GITHUB**




## Forking
A fork is a copy of a repository that allows you to freely experiment with changes without affecting the original project. A forked repository differs from a clone in that a connection exists between your fork and the original repository itself. In this way, your fork acts as a bridge between the original repository and your personal copy where you can contribute back to the original project using Pull Requests.

# How to fork
-->Go to repository, that you want to fork
-->on top right corner you will se a button 'Fork', click that
-->it will then ask, to which account you have to fork the repo. Select your prefferd account.

## Cloning
Cloning a GitHub repository creates a local copy of the remote repo. This allows you to make all of your edits locally rather than directly in the source files of the origin repo.
# -> $ git clone https://github.com/deepak2431/gitseries
# -> $ cd gitseries
-> This will clone the repo on local

## What is PR
PR--> PR stands for pull request, A pull/merge request is submitted when you’ve worked on some code from a particular branch and want to inform the others of the changes you’ve made. A person/people can be assigned to review and subsequently approve the request before your changes can be incorporated into the branch. Users can give their contributions in the world of open source projects.

## How to make a PR
Fork the Repository-->Clone the Repository-->Create a new branch [ master branch may also be used]-->commit ur changes localy-->Update ur local repo-->push the changes-->create the PR on github

## What is a branch
in layman's term we can say that git branches are individual projects within a git repository...all the branches are independant of each other. There is default 'Master' branch in git. Once we have made changes to a project we can merge that particular branch to the master branch. It is used mainly to reduce redundancy in the project

#How to make a branch
->Before creating a new branch, pull the changes from upstream. Your master needs to be up to date.
# ->$ git pull
# ->$ git checkout -b <BRANCH NAME>
-> This will create the branch
-> $ git push origin <BRANCH NAME>
-> This will push the branch in your repo,

## What are merge conflicts
)Merge Conflicts-->Conflicts generally arise when two people have changed the same lines in a file, or if one developer deleted a file while another developer was modifying it. In these cases, Git cannot automatically determine what is correct. Conflicts only affect the developer conducting the merge, the rest of the team is unaware of the conflict. Git will mark the file as being conflicted and halt the merging process. It is then the developers' responsibility to resolve the conflict.

There are two types of merge conflict 

🔵 During Start-->A merge will fail to start when Git sees there are changes in either the working directory or staging area of the current project. Git fails to start the merge because these pending changes could be written over by the commits that are being merged in. When this happens, it is not because of conflicts with other developer's, but conflicts with pending local changes. The local state will need to be stabilized using git stash, git checkout, git commit or git reset. 

🔴 During Merge-->A failure DURING a merge indicates a conflict between the current local branch and the branch being merged. This indicates a conflict with another developers code. Git will do its best to merge the files but will leave things for you to resolve manually in the conflicted files. 

# How to intensionaly create a Merge conflict!!
# ->$  mkdir git-merge-test
# ->$ cd git-merge-test
# ->$ git init .
# ->$ echo "Content" > merge.txt
# ->$ git add merge.txt
# ->$ git commit -am"we are commiting the inital content"

->Now we have a new repo with one branch master and a file merge.txt with content in it. Next, we will create a new branch to use as the conflicting merge.

# ->$ git checkout -b new_branch_to_merge_later
# ->$ echo "totally different content to merge later" > merge.txt
# ->$ git commit -am"edited the content of merge.txt to cause a conflict"

-->With this new branch: new_branch_to_merge_later we have created a commit that overrides the content of merge.txt
# ->$git checkout master
# ->$Switched to branch 'master'
# ->$echo "content to append" >> merge.txt
# ->$git commit -am"appended content to merge.txt"

-->This chain of commands checks out the master branch, appends content to merge.txt, and commits it. This now puts our example repo in a state where we have 2 new commits. One in the master branch and one in the new_branch_to_merge_later branch. At this time lets git merge new_branch_to_merge_later.

# ->$ git merge new_branch_to_

-->This will create a merge conflict

## What are issues?
Issues shown in github is the way to track the problems while using the code in repository. Anybody use the code can raise issues and responsible people will take it forward to fix the problem after verifying. It can also be used to keep track of tasks, enhancements for the code base.

## How to open an issue?
-->On GitHub Enterprise, navigate to the main page of the repository.
-->Under your repository name, click  Issues.
-->Click New issue.
-->Type a title and description for your issue.
-->If you're a project maintainer, you can assign the issue to someone, add it to a project board, associate it with a milestone, or apply a label.
-->When you're finished, click Submit new issue.
 
