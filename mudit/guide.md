# **GUIDE ABOUT GIT/GIT HUB**

**GIT :**

*Git is a ```distributed control version software``` i.e. it helps us to keep the record of the history in the form of remote and local repo(repository) so that we can access the history any time without any obstruction.Version control system means that it helps in  managing a project's source code. It helps in keeping track of changes made in a source code and repositories manages all the edits or changes. It is a open source tool and you can load the repositories in your local repository or in your local system as well.

**GITHUB :**

*GitHub is a ```website or web service``` which allows people to perform social coding which has version control on them i.e. Git*

###### NOTE: One dont need to know about both, one can eaily be oriented on GIT or GITHUB,and also one can work using both GIT and GITHUB too.

*Git has a work-flow, i.e. **```add-->commit-->push-->pull```***
1. Creating branch(by default master) and then creating the files and working on it.
2. adding the file(s) and commiting the file(s).
3. Merge your other branch if you have created any with master if your newly created branch worked perfectly or else modify.
The files will be stored in local and remote repo so that we can access our project anytime.



**Commit :**

*Commit is generally used to **save** the changes or edits in the local repository. Commit also generates a ```unique hash (ID)``` to the file as soon as you perform a change.*

**push/pull :**

*pushing is to send the file from your local system to local repository
pulling is to recieve the file.*

**Clone :**

*When you make a copy of remote repo in your local repo in the GIT is called cloning repository.*

*We perform cloning using ``` git clone```*

**Fork :**

*When you make a copy of remote repo in your local repo in the GITHUB is called forking repository.*

**Branch :**

*Branch is basically a part or version of repo. a single repo can have multiple branches and multiple branches can be merged into one as well.by defeault : Master branch.e.g. if we are working on project under master branch and suddenly we create another branch names X and continue the project, we can go back to that instance where we created branch Xi.e. working on branch will not affect other branches thus helping in creating and accessing the different versions of the projects.*

*We can create branch by both ways:-*

1. Using GITHUB, creating new branch and files under it, thus commiting new changes and later merging it with the other branch if you want.
2. Using ```git checkout -b name_of_branch```

**PR :**

*PR: **PULL REQUEST**, It let you tell others about changes you've pushed to a branch in a repository on GitHub. You can accept the PR if you want to implement the changes suggested.*

**Merge Conflict**

*Conflicts generally arise when two people have changed the same lines in a file, or if one developer deleted a file while another developer was modifying it. In these cases, Git cannot automatically determine what is correct. Conflicts only affect the developer conducting the merge, the rest of the team is unaware of the conflict.*

