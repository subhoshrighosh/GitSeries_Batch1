Complete guide about git and github.
---------------------------------------------------------------------------------
Q1. What exactly do u mean by Git and github ?
Ans.Git is a popular control system which is installed and it maintains all your 
local system and gives you a self contained record if your ongoing programming 
versions. Git is easy to learn and has a tiny footprint with lightning fast 
performance. It outclasses SCM tools like Subversion, CVS, Perforce, and ClearCase 
with features like cheap local branching, convenient staging areas, and 
multiple workflows.Git is written in CC, Perl, Tcl, Python. The original author is
Linus Torvalds. Best part about Git is that you dont need internet connection to 
access it and its is free of cost and easy to use. 
GitHub is designed as a Gut repository hosting service. Git repository hosting is 
an online database that allows you to keep track of your work and shares your 
Git projects outside the local server. It is popular for open source projects. 
If the server is failed then the data is not lost since it is saved in your 
local repository.The parent organisation of github is Microsoft Corporations.
It was founded in 2008 and the CEO of github is Nat Friendman. Github is written 
in Ruby. Github has a total of 40 million user by Aug 2019. Founder of github are
Tom Preston-Werner, P.J Hyett, Chris Wanstranth, Scott Chacon.

Q2. Why Github is so popular in most of the projects? 
Ans. 
a. The Largest shared repository- Pushing the project to a shared, public repository
 makes it instantly discoverable for those 28M users.
b. Easy Version Control- It tracks all the changes made to your code and who makes them.
c. Immensely Powerful Community-itHub is an open-source platform, and the community is really
that fills it up.
d. Secure Cloud storage-The platforms protect all your data for you: protects code branches, 
verifies commit signing, controls access. 

Q3.What are the other platforms similar to Github?
Ans. 
a.GitLab
b.Google cloud source repositories 
c.AWS Code commit 
d.Apache Allura 

Q4. Q1 How git workflow works?What are the different stages of a git 
the project as commit, add?
Ans.
1. Working directory - Workspace.
2. Index ie stage
3. Local Repository ie Head
4. Remote Repository
There is one central repository. 
Each developer clones the repo,
works locally on the code,
Modifies and makes the changes as required
Commit the changes using command commit -a with changes
and push it to the central repository 
for other developers to pull and use in their work.

Q5.Is it possible to do a git commit before git add .
If you have made any changes? Explain why?
Ans. No, because according to the process
first, we have to add the file and then commit changes to it
After making the changes we will add them using "git add ."
and then we can commit it using (commit -a).

Q6. Why is git diff used?
Ans. git diff is used to track the difference between the changes made on a file. This command shows all the
changes which are done. Diff command takes two inputs and 
reflects the differences between them. It is not necessary
that these inputs are files only. 
It can be branches, working trees, commits and more. 

Q7.Can we leave the commit message as blank?
Ans. git commit -a --allow-empty-message -m ""
It is a valid request,commit can have no message at all.

Q8.What do you mean by fork and clone ?
Ans. Fork - We create a copy of the main repository of a project s
ource code to our own github profile. In this we can do any changes 
without affecting the main source of the project. Fork repository 
makes a connection between our fork and the original repository and we
can go back to the original project using pull request. 
We do clone to make our own repository on our local computer. 
We cannot pull the changes from the original repository when clonning. 

Q9.What are branches in Github ?  What is PR ? 
Ans. When we create a repository, then the main linear list of 
commits are on master branch. We can makes changes in master as well 
as in a new branch. All the branches are independent of each other. 
After editing we can commit the changes in the branch directly or create 
a new branch. 
PR stands for pull request. 
It lets others know about the changes we have pushed to a branch in 
a repository of github. Once the pull request is open we can discuss 
and review it before the changes are merged into the main brach. 

Q10. Can we delete the mastar branch if not why?How can we delete the master branch ?
Ans.Yes we can delete the master branch. 
First delete the master in your local clone. We can make a new branch 
first and delete the master. 
We cannot delete the master branch directly from github instead first we 
will make github look for our new branch and then delete the master branch. 
To do so we will push the new branch then set the new branch to github default 
branch then go to main github page for your forked repository and click on 
admin button and you are done its set as default. 

Q11. What do u mean by merge conflict? 
It occurs when git is is unable to automatically resolve the differences 
in the code by itself between two commits. When there is a conflict git 
doesn’t know which code to keep and which to discard. For eg if there is 
conflicting changes on the same line or some file is deleted on one branch 
but not on other. Merge conflict can only be resolved by the developer. 
These conflict usually happens when working in a team environment. 
Command for merge is 
"git mearge branch_name"

a. Git fails to start the merge when there are changes in the working directory 
or staging area of current project.
b. Git fails during merge - conflict in current local branch and branch being
merged. 


Q12. Can we have 200 different branches other than the master ? 
Ans. Yes we can have 200 different branches other than the master.

Q13. What is the difference between git branch -d and git branch -D ? 
Ans. git branch -d is the command use to delete a branch. The branch 
must be fully merged in its upstream. 
"git branch -D is the shortcut command for - - delete - - force"

I hope this solves your questions and you all can have a look at my github
I am sharing the link below:-
https://github.com/priya8936

Enjoy..!! 
Github is really fun to use and i would like to thank my mentors in guided me 
through this whole process.
Thank you
Regards
Priya Aggarwal


