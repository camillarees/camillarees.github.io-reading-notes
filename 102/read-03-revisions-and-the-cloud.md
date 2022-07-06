# Revisions and the Cloud - Notes Outline

## Version Control

A system that allows you to: 
- Revisit various versions of files by recording changes
- Revert a files to a previous version
- Track modifications 
- Easily fix mistakes

### Local Version Control (VCS)

A Local VCS entails one database on your hard disk that stores changes to files

### Centralized Version Control (CVCS)

A single server system that:
- Stores all changes and file versions
- Allows multiple client access
- Allows programmers to see team members’ activities with files
- Gives administrators control over revision privileges

### Distributed Version Control (DVCS)

- Allows clients to create mirrored repositories to save backups and replace lost information
- Allows colaboration on joint projects through the enablement of various simultaneous workflows

### What is Git?

**Snapshots**

- Git is a DVCS that stores data in a system made up of snapshots
- Each time you commit (save) a changed version of your project, Git creates and stores a snapshot of the file

**Local Operations**

1. Git relies on local operations which:
  - Allows for process expediency because a project’s history resides on the local disk
  - Eliminates the need to fetch history information from the server so you can keep working on a project when not online or on a VPN

**Tracking Changes**

- Git tracks every every change applied to any file or directory
- As the gatekeeper, Git will detect file corruption or loss of information in transit

**Loss of Data**

- Git makes it almost impossible to lose or damage a snapshot of a committed file, or to lose data in general

**States**

Files in Git resides in 3 main states:

 1. Committed
    - Data is stored in local database
 2. Modified
    - File has been changed but not committed to database
 3. Staged
    - File’s changed version is flagged to be committed in the next snapshot

## Getting Started

### Download Git

-  Make sure your computer has Git available and that you get the latest version 

**Git can be installed in 3 ways:**

1. As a package
2. Via another installer
3. Download and compile the source code

### Mac OS X

1. Terminal (simplest on Mac)
2. Git Website: Use link: http://git-scm.com/download/mac
3. GitHub: Install Git as part of the GitHub for Mac install: http://mac.github.com

### Windows

1. Git Website: Use link: http://git-scm.com/download/win
2. GitHub: Install Git as part of the GitHub for Windows install: http://windows.github.com

### Linux

1. Package Manager
  - Fedora: $ sudo yum install git
  - Ubuntu: $ sudo apt-get install git
2. Git Website: Use link: http://git-scm.com/download/linux

### Graphical Clients

Git includes inherent Graphical User Interface (GUI) tools. 

**GUI Clients**

Access a variety of GUI clients for Mac, Windows, and Linux: https://git-scm.com/downloads/guis

### Initial Customization

After Git is installed: Perform customization steps  

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
- To configure a different text editor, such as Emacs, type into Terminal or Command Line: $ git config --global core.editor emacs

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

To import an existing project or directory, use the Terminal or Command Lines:

```
$ cd test (cd = change directory)
Use the git init command
$ git init
```

This switches to the target project’s directory and creates new subdirectory named .git that has repository files

```
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”
```

### Cloning

To make a copy of a Git repository from a server, use the clone command with a repository’s URL: $ git clone https://github.com/test

Clone a repository into a directory with another name by using command format: $ git clone https://github.com/test mydirectory

## Workflow

### Local Repository Structure

The local Git repository has 3 successive components:

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

Untracked files do not reside in the staging are since they were not in the last snapshot

### The Life Cycle of File Status

- Git flags edited files as modified 
- You stage the modified file
- You commit staged changes

### Check File Status

To determine the state of files, use the git status command: $ git status

### Tracking and Staging a New File

- Track one file only: git add filename

- Track all files in a repository: $ git add *

### Committing a File

Commit changes to staged files and record changes within the commit message: $ git commit -m “made change x,y,z”

### Committing All Changes

Commit a snapshot of all modifications in working directory: $ git commit -a

### Pushing Changes

Example of pushing changes (from local master brance to remote repository named "origin": $ git push origin master
             
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

- To view short names of specified remote handles, such as "origin", run git remote command 
- To view all remote URLs next to their short names, use git remote -v

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
