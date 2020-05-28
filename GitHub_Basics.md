# GITHUB



## What is Git and Github?

Git is Distributed Version Control System.This means that every user will have their own copy of program at their local repository along with having it on the remote repository.It is free and open source.


Github is a web service which implements the remote repository.So wecan save our work on github.


## Workflow of Git

Git workflow consists of:
- Workspace(Working Directory)
- Index (Stage)
- Local Repository(HEAD)
- Remote Repository 


     - clone command creates a local copy of the repository in the workspace/working directory.



     - add command adds the file from workspace to the Index.



     - commit command saves the file in the local repository 



      Note: commit -a command does the both work of add and commit command.



     - push command saves the file from local to remote repository.



      Now the reverse process goes like this:



     - fetch command gets the file from remote to local repository.



     - merge command gets your file from local tow workspace.



     - pull command takes the file directly from remote repository to workspace.





## Some Important Terminology in Github

- Cloning

  As already defined above cloning is a process to create a local copy of the repository in the workspace.

  On Github whenever we open our account(or reposiotory) or anyone's profile 

  then there is "Clone or Download" option with green tab.

  Steps for cloning:
  
   - We need to "click clone and download" button if we want to save that file in our workspace.

   - After clicking we need to copy the link which it shows there.
  
   - Then open Git Bash on our PC.
   
   - On Git Bash Terminal change the directory using cd command wherever you want to save your cloned file.
   Commands to change the directory to Desktop
   ```
   cd ~
   cd ..
   cd <PC USER>
   cd Desktop
    ```
   - On Git Bash Terminal write "git clone <URL which you copied>
     To clone
     ```
     git clone https://github.com/your-username/repository.git
     ```
     To change the directory to the cloned repository
     ```
     cd repository
     ```
     To create a new branch named new-branch
     ```
     git branch alpha
     ```
     To switch to the newly created branch named new-branch
     ```
     git checkout new-branch
     ```
     To add file abc.txt 
     ```
     git add abc.txt 
     ```
     To save the changes to the file
     ```
     git commit -m "Initial Comment"
     ```
     To know about which branch you are working on and other details
     ```
     git status
     ```
     To push your files to Github
     ```
     git push --set-upstream origin new-branch
   ```
   - Now cloning and pushing has been done and the file is saved on your PC.

- Forking

  Forking means creating a personal copy of someone else's project and modifying it.

  Someone else's project can be used as the beginning of someone else's project.

  Steps for forking

    - Open the profile of the person(the location of the file to be forked) from whom you want to fork the file.
    
    - There you need to select the "Fork" button which is situated at the top right column.

    - Now after forking follow the cloning steps.



- Pull Request

  Pull Request allows others to know about the changes one has pushed in the github repository.

  A Pull Request is submitted when you’ve worked on some code from a particular branch and want to inform the others of the changes you have made.

  So after forking a project we can pull request.

  Steps for creating PR:

    - After forking and cloning the project or file to your locall sysytem, you need to work on Git Bash.
    
    - Make the changes you want to in the cloned file uing git commands.
    
    - After modifying, you need to push it on github using "git push" command

    - Give your userid and password to the prompt window.
   
    - On github, Click on "Compare and Pull Request button.

    - Click on "Create pull request to open a new pull request.



- Creating Issues on Github
  
  Issues are used to keep track of bugs, enhancements, or other requests.

  Steps to create an Issue:

    - Go to the main page of the repository.

    - Click on Issues.
    
    - Click on New Issue.
  
    - Type the title and description for the issue, can also use labels.

    - Click on Submit new issue.  


----------------------------------------------------------------------------------------------------------------------------------------
