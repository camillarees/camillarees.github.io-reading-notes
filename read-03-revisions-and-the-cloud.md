# Revisions and the Cloud - Notes Outline

## Version Control

A system that allows you to: 
- Revisit various versions of a file or set of files by recording changes
- Revert a file or project to a previous version
- Track modifications and modifying individuals 
- Easily rectify mistakes

### Local Version Control (VCS)

A Local VCS entails one database on your hard disk that stores changes to files

### Centralized Version Control (CVCS)

- A single server system that stores all changes and file versions
- Allows multiple clients access
- Allows programmers to have more knowledge of team members’ activities with certain files
- Gives administrators more control over divvying up revision privileges

### Distributed Version Control (DVCS)

- Allows clients to create mirrored repositories to save backups to replace lost information
- Allows programmers to collaborate on joint projects through the enablement of various simultaneous workflows

### What is Git?

**Snapshots**

- Git is a DVCS that stores data in a file system made up of snapshots
- Each time you commit (save) a changed version of your project, Git creates a snapshot of the file and stores a reference to it
- If the file has not changed, Git only stores a reference to the already-stored identical version of it

**Local Operations**

1. Git relies on local operations which allows for process expediency because a project’s history resides on the local disk
  - This eliminates the need to fetch history information from the server
     - This allows continued work on a project even when not online or on a VPN.

**Tracking Changes**

- Every change applied to any file or directory is tracked by Git
- As the gatekeeper, Git will always detect file corruption or loss of information in transit

**Loss of Data**

- Git minimizes the possibility of irreversible damage to files, such as accidentally lost data
- It's almost impossible to lose a snapshot of a committed file

**States**

Files in Git can reside in three main states: committed, modified and staged.

 1. Committed
    - Data is securely stored in a local database
 2. Modified
    - File has been changed but not committed to the database
 3. Staged
    - Flagged a file’s changed version to be committed in the next snapshot

## Getting Started

### Download Git

- In order to use Git, your computer must have it available
- Make sure you have the latest version.

**Git can be installed in three ways:**

1. Install as a package
2. Install via another installer
3. Download and compile the source code.

### Mac OS X

1. Terminal (simplest on Mac)
2. Git Website
  - Use link: http://git-scm.com/download/mac
3. GitHub
  - Install Git as part of the GitHub for Mac install: http://mac.github.com

### Windows

1. Git Website
  - Use link: http://git-scm.com/download/win
2. GitHub
  - Install Git as part of the GitHub for Windows install: http://windows.github.com

### Linux

1. Package Manager
  - Fedora:$ sudo yum install git
  - Ubuntu: $ sudo apt-get install git
2. Git Website
  - Use link: http://git-scm.com/download/linux

### Graphical Clients

Git includes inherent Graphical User Interface (GUI) tools. 

**GUI Clients**

Access a variety of GUI clients for Mac, Windows, and Linux: https://git-scm.com/downloads/guis

### Initial Customization

After Git is installed:
- Perform customization steps which should only need to be completed once on any machine

**Configuration of Variables**

git config: Allows the setting of configuration variables that control aspects of Git’s operation and look

**Identity Setting**

- Set the user name and email address
- Type into Terminal or Command Line:

```
git config --global user.name "Jane Smith"
git config --global user.email "example@email.com"
To confirm that you have the correct settings, enter the following command:
git config --global user.name (should return Jane Smith)
git config --global user.email (should return example@email.com)
```
-  –global: applies settings to anything on the system
-  For specific project settings, don't use -global 

### Default Text Editor

- Default Text Editor is Vim
- To configure a different text editor, such as Emacs, type into Terminal or Command Line:

```
$ git config --global core.editor emacs
```

### Check Settings

To check settings, use the git config --list command.

```
Example:

$ git config --list
user.name=Jane Smith
user.email=example@email.com
color.status=auto
color.branch=auto
color.interactive=auto
```

### Getting Help

Ways to get information on commands:

1. git help command
2. git command --help
3. man git-command


## Setting up a Git Repository

### Importing

To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

1. Switch to the target project’s directory and created new subdirectory named .git that has the repository files.

```
Example:

$ cd test (cd = change directory)
Use the git init command
$ git init
```
2. Track these repository files, perform an initial commit by typing:

```
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”
```

### Cloning

Create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

```
$ git clone https://github.com/test
```

"test" will have copies of all versions of all files for the specified project

Clone a repository into a directory with another name by using command format:

```
$ git clone https://github.com/test mydirectory
```

## Workflow

### Local Repository Structure

The local Git repository has three successive components:

1. Working Directory: Where files reside
2. Index: Area used for staging
3. Head: Points to the most recent commit

### Saving Changes

**Tracked State File:**

Since they were in the latest snapshot, tracked files can be:
- Modified
- Unmodified
- Staged

**Untracked State File:**

Untracked files were not in the last snapshot and do not currently reside in the staging area

### The Life Cycle of File Status

- Git flags edited files as modified 
- You stage the modified file
- You commit staged changes

### Check File Status

To determine the state of files, utilize the git status command:

```
$ git status
```

### Tracking and Staging a New File


- Track one file only:

```
git add filename
```

- Track all files in a repository:

```
$ git add *
```

### Committing a File

Commit changes to staged files and record changes within the commit message:

```
$ git commit -m “made change x,y,z”
```

### Committing All Changes

Commit a snapshot of all modifications in working directory

```
$ git commit -a
```

### Pushing Changes

Example of pushing changes (from local master brance to remote repository named "origin":

$ git push origin master
             
### Stashing Changes

- Stash changes: Temporarily hide changes

## Remote Repositories

- Versions of a project residing online or on a network
- Read/write privileges only
- Teams can use remote repositories to push information to and pull data from

### Cloned Repositories

- Cloned repositories automatically named "origin"
- Local branch named "master" 

### Seeing Your Remotes

- By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles
- By using git remote -v, you can view all the remote URLs next to their corresponding short names.

```
$ cd example
$ git remote -v
remote1 https://github.com/remote1/example (fetch)
remote1 https://github.com/remote1/example (push)
remote2 https://github.com/remote2/example (fetch)
remote2 https://github.com/remote2/example (push)
remote3 https://github.com/remote3/example (fetch)
remote3 https://github.com/remote3/example (push)
```
