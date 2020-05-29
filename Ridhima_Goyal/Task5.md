## Git and GitHub

Git is a distributed version control tool that can manage a development project's source code.
Git is an Open Source Distributed Version Control System.
Git also tracks the history of changes to a project’s source code including what specifically has been changed and who has 
changed what parts and when have they been changed, this feature is termed as Version Control.

GITHUB:-

GitHub is a open source platform built around the Git tool.
It allows developers to host their files in a Repository, so that others can collaborate and make suggestions on projects.
A GitHub repository can be used to store a development project.Git is a distributed version control tool that can manage 
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
## Forking and Cloning

Fork in git means making a personal copy of others repository which we can modify
without affecting the orignal project.

Clone is used to create  a local copy of the remote repository.This process helps us to edit and modify files locally.
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
-----------------------------------------------------------------------------------------------------------------------------------------
## Merge Conflict

Conflicts arise when two people have changed the same lines in a file, 
or if one person deleted a file while another person was modifying it. 
In these cases, Git cannot automatically determine what is correct. 
Git will mark the file as being conflicted and halt the merging process. 

