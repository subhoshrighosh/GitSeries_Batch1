#**Guide For Github**

### How github works:
GitHub is a file or code sharing service to collaborate with different people. 
GitHub is a highly used software which is used for version control. It is helpful when more than just one person is working on a project.Github helps various users to build a centralized repository where everyone can upload, edit and manage the code files. 
GitHub is a central repository and Git is a tool which allows you to create a local repository.Git is a version control tool that will allow you to perform all kinds of operations to fetch data from the central server or push data to it whereas GitHub is a core hosting platform for version control collaboration. GitHub allows you to host a central repository in a remote server.

***GitHub  Workflow:***

**1. Workspace:**
The Workspace is the area where we are currently working. It is where our files are stored. If we make changes to files in your workspace git will recognize that they are modified.To know what is stored in our file: Run the command git status. This command will show you two things: The files in your Workspace and the files in your Staging Area. 

**2. The Staging Area (Index):**
The Staging Area is when git starts tracking and saving changes that occur in files. These saved changes reflect in the .git directory. If you want to track specific files, then git moves from Workspace to the Staging Area. If you make any more additional changes after adding a file to the Staging Area, git will not know about those specific changes until you tell it to see them. We explicitly have to tell git to notice the edits in our files. To know which files are in staging area click git status.

To add files to the Staging Area: Run the command (git add filename) will add a specific file to the Staging Area from your Workspace. If we want to add everything from the Workspace, then run the command (git add . ). The . operator is a wildcard meaning all the files from the workspace are staged in the stagin area.

**3. The Local Repository:**
The Local Repository is everything in our .git directory. Mainly what we will see in your Local Repository are all of our checkpoints or commits. It is the area that saves everything.

To add items from our Staging Area to our Local Repository: The git command git commit takes all changes in the Staging Area, wraps them together and puts them in our Local Repository. A commit is simply a checkpoint telling git to track all changes that have occurred up to this point using our last commit as a comparison. After committing, your Staging Area will be empty.

**4. Remote Repository:**
As we make changes to our project locally on our system, we can keep them up-to-date with our remote repository. In Git, a remote is the server where our code is stored. In our case, that server is a repository on GitHub.


### Cloning:
When we create a repository on our GitHub Server, it exists as a remote repository. Anyone can clone our repository (if it has public access) to create a local copy on their computer and sync between the two locations.

On GitHub, navigate to the main page of the repository. Under the repository name, click Clone. In the Clone with HTTPs section, click  to copy the clone URL for the repository. Clone URL button. Open Git Bash terminal. Change the current working directory to the location where you want the cloned directory to be made.Type git clone, and then paste the URL you copied. After it, Press Enter. Your local clone will be created on your system.
 

### Forking:
A fork is a copy of a repository. Forking a repository allows us to freely experiment with changes without affecting the original project. Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for our own idea.

A great way of using forks to propose changes is for bug fixes. Rather than logging an issue for a bug you've found, you can:
Fork the repository. Make the fix. And then submit a pull request to the project owner.If the project owner likes your work, they might pull your fix into the original repository!



### Making Pull Requests:
Pull requests tell us others about changes we've pushed to a branch in a repository on GitHub. Once a pull request is opened, we can discuss and review the potential changes with collaborators and add follow-up commits before our changes are merged into the base branch.

After initializing a pull request, we'll see a review page that shows a high-level overview of the changes between our branch (the compare branch) and the repository's base branch. We can add a summary of the proposed changes, review the changes made by commits and add labels.

Once we've created a pull request, we can push commits from our branch to add them to our existing pull request. These commits will appear in chronological order within our pull request. Other contributors can review our proposed changes, add review comments, contribute to the pull request discussion, and even add commits to the pull request. After we're done with the proposed changes, we can merge the pull request. If we're working in a shared repository model, we create a pull request and someone else, will merge your changes from our branch into the base branch you specify in your pull request.We can link a pull request to an issue to show that a fix is in progress and to automatically close the issue when someone merges the pull request. 


### Opening issues:
To contributing to a project we may find an issue on which we would like to work on and which we think is suitable for our skill set. Many projects labels their issues and we can work on it. Issues can be raised by anyone. It can also be raised by us.

When beginning work on an issue locally, the first thing we’ll need to do is to create a branch for that piece of work on which we'll work.Once we are on our new branch we can make changes to the code which address the issue. To resolve the issue we can made the required changes that address a particular issue, we need to commit that code to our branch. We can use the (git status) command to view the changes since our last commit. We then use the (git add) command to stage the changes for the next commit and then use the commit command with a message to specify what is committed through us in the file.

Now that we have made and committed out changes local to our development machine. Our final step is to push the changes to our fork of the repository up on GitHub. We can do that using the (git push) command. We need to specify the name of the remote that we want to push to and the name of the branch we want to push up.