# Class 3 Notes - How to use Git and GitHub

[Back to Home](../README.md)

Awesome Resource: [Git Tutorial](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)

To explain Git, we have to first explain various aspects of Version Control.

Distributed Version Control System

+ Overcomes the lack of cooperation with local version control
+ single point of failure with centralized Version Control.

Git is a DVCS that stores data in a file system made up of snapshots.  
 Each time you save it is a "Commit."  

commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, 
Git only stores a reference to the already-stored identical version of it.

Local Operations
+ Git mostly relies on local operations because most necessary information can be found in local resources. 
+ This allows for process expediency because a project’s history resides on the local disk, eliminating
the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.

Tracking Changes
Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, 
Git will always detect file corruption or loss of information in transit.

States
Files in Git can reside in three main states: committed, modified and staged.
Committed- Data is securely stored in a local database
Modified -File has been changed but not committed to the database
Staged -Flagged a file’s changed version to be committed in the next snapshot

**Linus Torvalds** - Linux and Git - he is awesome. Git is the best.


Initial Customization

After making sure Git has been installed, you should perform some customization steps, which should only need to be completed once on any
machine. To change settings, you can repeat these steps. 

Configuration of Variables  
An inherent Git tool called git config allows the setting of configuration variables that control aspects of Git’s operation and look. 

  Identity Setting  
After installing Git, users should immediately set the user name and email address, which will be used for every Git commit.  

  Type the following into Terminal or Command Line:  

git config --global user.name "Jane Smith"  
git config --global user.email "example@email.com"  

  To confirm that you have the correct settings, enter the following command:  
git config --global user.name (should return Jane Smith)  
git config --global user.email (should return example@email.com)

  *By using the –global option, these Git settings apply to anything on the system. To use different identity settings for
a specific project, change the working directory to the desired local Git repository and repeat the steps above without using –global.

  Default Text Editor  

Without configuration of a default text editor, Git will use the system’s default editor–most likely Vim.
To configure a different text editor, such as Emacs, type the following into your Terminal or Command Line:
$ git config --global core.editor emacs

  Check Settings  
To check settings, use the git config --list command.

  Getting Help  
There are three ways to get more information on a particular command, by accessing the manual:
git help command
git command --help
man git-command



### Setting up a Git Repository
  Importing
To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

Switch to the target project’s directory
Example:

'$ cd test (cd = change directory)'  

Use the git init command
'$ git init'
Note: At this stage, you have created a new subdirectory named .git that has the repository files. Tracking has not commenced.

To start tracking these repository files, perform an initial commit by typing the following:
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”
Now, your files are tracked and there’s an initial commit. We will discuss the particular commands in detail soon.


  Cloning
You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

$ git clone https://github.com/test
By cloning the file, you have copied all versions of all files for a project. This command leads to the creation of a directory called “test,” with an initialized .git directory inside it, which has copies of all versions of all files for the specified project. The command also automatically checks out — or retrieves for editing — a copy of the newest version of the project.

To clone a repository into a directory with another name of your choosing, use the following command format:

$ git clone https://github.com/test mydirectory
The command above makes a copy of the target repository in a directory named “mydirectory.”


  Workflow
Local Repository Structure
The local Git repository has three components:

Working Directory: The actual files reside here.
Index: The area used for staging
Head: Points to the most recent commit
image03

  Saving Changes
All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.

Tracked - Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

Untracked - Untracked files were not in the last snapshot and do not currently reside in the staging area.

*After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.

   The Life Cycle of File Status
After you edit a file, Git flags it as modified because of changes made after the previous commit.
You stage the modified file.
Then, you commit staged changes.

And so much more... go to the link at the top of the page.

