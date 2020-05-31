1.How github works?
	GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.
Working of github is very simple at first developers start it by cloning the central repository. In their own local copies of the project, they edit files and commit changes as they would with SVN; however, these new commits are stored locally - they’re completely isolated from the central repository. This lets developers defer synchronizing upstream until they’re at a convenient break point.
To publish changes to the official project, developers "push" their local master branch to the central repository. This is the equivalent of svn commit, except that it adds all of the local commits that aren’t already in the central master branch.

2.What is cloning and forking?
	 Clone a repository or cloning a repository is downloading a copy of the source code from source control.fork a repository or forking a repository means  we create a copy of the original repository (upstream repository) but the repository remains on our GitHub account.
GitHub won't let you push code to repositories that you don't own or have sufficient permission to, you need to make a copy of the repository by forking it, and then you can make all your changes to that repository.
Once you have all the changes you want in your repository you can create a inaudible request to the project, and the maintainer can merge your changes into the main project. To do this we'll click on the fork button, and this will open up a dialog where we can click on our user to fork the repository to our users' repositories.
With that finished, we now have our own copy of the repository, this is forked from the egghead.io GitHub organization, but it's a part of our user, so we can make all changes to it that we want.
Now we need to take this SSH URL, and we'll copy it to our clipboard. Then we'll open our terminal, or if you're on a windows machine use GitBash, and git clone this repository into a directory where we want to edit the project.
Let's make sure that we're cloned the right project. If we LSAL, then we're going to see that we have a git, a gitignore, all of the files that this project has itself, so we're on the right track.
One of the challenges with forking a repository is keeping your copy up-to-date with the original repository, or the upstream repository. We're going to add the original repository as a git remote, so we can easily fetch and pull from it.
To do this we're going to need the SSH URL for the original repository. We'll go back to the main project here, we'll make a copy of the original SSH URL, and go into our terminal again, and we'll execute the command git remote add upstream and then paste the SSH URL that we just copied.
Now that we have the remote added, we need to tell our local git to go get information about that upstream remote, so we'll execute the command git fetch upstream. That will give us information about that remote.
It has a branch called master, and that is being pointed to upstream/master. Right now our local copy of the master branch is pointing to our personal remote repository. Our repository is called origin, we want our local copy of master to point upstream, so whenever we pull changes into master it will get the latest changes from the upstream repository.
To do this, we'll run the command git branch --set-upstream-to=upstream/master master. Now our branch, called master, is tracking the upstream master. When there are updates we like to get from the upstream repository we can get them by simply pulling on that branch.
We're now ready to set up our environment and the project for making our change.

3.How to make PR's?
	Find a project you want to contribute to.
1. Fork it.
2. Clone it to your local system.
3. Make a new branch.
4. Make your changes.
5. Push it back to your repo.
6. Click the Compare & pull request button.
7. Click Create pull request to open a new pull request.	

4.Opening issues=>The first step when contributing to a project is to visit the project site and find an issue you would like to work on and which you think is suitable for your skill set.
		  From the project homepage on GitHub you can click the Issues tab to navigate to a list of the open issues.
