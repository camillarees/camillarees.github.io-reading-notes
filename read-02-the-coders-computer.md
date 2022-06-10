# Choosing a Text Editor - Notes Outline

## What is a Text Editor?

- A text editor is pretty self-explanatory. It allows you to write and edit/manage text, particularly website content.
- It can either be software or online

### Important features to consider when selecting a text editor

1. Code completion: This predicts text and offers autofill suggestions, including catching mistakes like closing tag
2. Syntax Highlighting: Colorizes text to distinguish attributes, elements and copy.
3. Themes: A variety of themes reduces eye strain and fatigue
4. Extensions: Is there a healthy selection of extensions available when you need them? 
5. What are your must-haves?

### Why Third Party Options are Better than the text editors that come with your computer
- They almost always have more of the helpful features listed above.

1. Emmet: Speeds up code writing
2. NotePad++
  - Free text editor for Windows Computers only.
  - Has syntax highlighting and code, word and function completion
  - Has its own online community
3. BB Edit
  - Costs $
4. Visual Studio Code
  - Free text editor for Windows, Macs and Linux
  - Created by Microsoft.
  - Has the Emmet shorthand for HTML and CSS already built-in 
  - Has syntax highlighting, themes, extensions and code completion
5. Atom
  - Free text editor for Windows, Macs and Linux 
  - Created by GitHub
  - Has syntax highlighting, themes, extensions, etc. 
6. Brackets
  - Free text editor for Windows, Macs and Linux 
  - Created by Adobe
  - Only supports HTML, CSS and JavaScript
  - More coding capabilities can be added through extensions 
7. Sublime Text
  - Costs $ 
  - Fast and responsive
  - Has syntax highlighting, code completion,themes and extensions 

### What is an IDE?

- An IDE (Integrated Development Environment) is a text editor, a file
manager, a compiler, and a debugger all in one software package
- Similar to Microsoft Outlook (email, calendar, task manager, etc.)

## The Command Line

- A command line or terminal is a text based interface to the system
- It's called a command line because you mostly make text commands for the system to perform tasks or give feedback based on those commands
- If a prompt is displayed, the task is complete and it's ready for the next command
- If there is no prompt displayed, the system is most likely running the task

### How to Use a Command Line

**Opening a terminal**

- Mac: Find Terminal under Applications -> Utilities **or** 'command + space' for Spotlight to search Terminal
- Linux: Find Terminal under Applications -> System or Applications -> Utilities **or** 'right-click' on the desktop to 'Open in terminal'
- Windows: Use SSH client like Putty

**The Bash, Shell**

- Shell defines how the terminal will behave and looks after running (or executing) commands
- Most common shell is bash which stands for Bourne again shell
- Use echo command to display messages and see which shell you're using

**Shortcuts**

- Command are stored in a history
- Traverse this history using the up and down arrow keys
- Edit these commands using the left and right arrow keys to move the cursor
- ~ (tilde): Shortcut for your home director
- . (dot): Reference to your current directory. 
- .. (dotdot) Reference to the parent directory

## Basic Navigation

**Commands**

1. pwd: Print Working Directory. Tells you what your current working directory is
2. cd: Change Directories
3. file: obtain information about what type of file a file or directory is.
4.  ls: List. 
  - ( -l ): Long listing.
    - First character indicates whether it is a normal file ( - ) or directory ( d )
    - Following characters are permissions for the file or director
    - It also includes file size, modification time, and file name
  - ( ls -a ): List the contents of a directory, including hidden files.
5. Run with command line argument ( /etc ), it tells ls to list directory contents
6. Run with both command line option and argument for long listing of the directory

**Paths**

A path is a means to get to a particular file or directory on the system

- Absolute Paths: Specify a location (file or directory) in relation to the root directory. They always begin with a forward slash ( / )
- Relative Paths: Specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash
- Root Directory: ( / ). Made up of subdirectories containing files

## More About Files

**Linux**
- Everything is a file
- An extensionless system
- Case sensitive

**Common Extensions**

- file.exe - an executable file, or program
- file.txt - a plain text file
- file.png, file.gif, file.jpg - an image.


