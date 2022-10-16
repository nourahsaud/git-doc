# A Simple Git Explanation

![Git-Logo](https://wac-cdn.atlassian.com/dam/jcr:f6948a92-f446-466f-8783-1dd1cbcc661a/hero.svg?cdnVersion=578)

## What is Git and Why we need it?
Git is a version control system [(VCS)](a "Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.") that developers use all over the world. It helps you track different versions of your code and collaborate with other developers.
Git helps you to track of which changes were made, by whom, and when those changes were made. 
----

## The three States
###### Git has three main states that your files can reside in: modified, staged, and committed
- Modified (Working directory) means that you have changed the file but have not committed it to your database yet.
- Staged (index) means that you have marked a modified file in its current version to go into your next commit snapshot.
- Committed (Git directory (Repository)) means that the data is safely stored in your local database.

![Workflow](https://miro.medium.com/max/1400/1*zw0bLFWkaAP2QPfhxkoDEA.png)
____________________________________________________________________________
The basic Git workflow goes something like this:
1. You modify files in your working tree.
2. You selectively stage just those changes you want to be part of your next commit, which adds
only those changes to the staging area.
3. You do a commit, which takes the files as they are in the staging area and stores that snapshot
permanently to your Git directory.
-----
## Installing Git
In order to check if you already have Git installed on your computer you can type the command `git --version` in the terminal.

If you already have Git installed then you will see what version you have. If you don’t have Git installed you can visit the [Git website](https://git-scm.com/downloads) and easily follow the download instructions to install the correct version for your operating system.

---
## Git Basics 

   ## Tutorial
   ### IMPORTING A NEW PROJECT
   `$ mkdir project`
   `$ cd project ` 
   `$ git init `
   Output 
   -` Initialized empty Git repository in .git/ `
   + You’ve now initialized the working directory—you may notice a new directory created, named ".git".
       
    > Next, tell Git to take a snapshot of the contents of all files under the current directory (note the .), with git add:
    `$ touch <new-file.ex>` 
    `$ git add .` 
    
    This snapshot is now stored in a temporary staging area which Git calls the "index". You can permanently store the contents of the index in the repository with git commit:
   
    `$ git commit`
    `$ git commit -m 'added a nwe file'`
    
    This will prompt you for a commit message. You’ve now stored the first version of your project in Git.
    
       
     ### VIEWING PROJECT HISTORY 
      At any point you can view the history of your changes using

           `$ git log`
           
    
    ### MANAGING BRANCHES
       A single Git repository can maintain multiple branches of development. To create a new branch named "experimental", use `$ git branch` 
       
       If you now run
       `$ git branch newbranch`
       `$ git branch `
        Output 
            `* master`
            `newbranch`
        `$ git checkout -b <name-file> `
        Output 
            ` master`
            `* newbranch`

        `$ git merge <branch-name> `
        fast-forword 
        3-way merge
        
        
Branch in Git

Branch in Git is used to keep your changes until they are ready. You can do your work on a branch while the main branch (master) remains stable. After you are done with your work, you can merge it with the main office.

The above diagram shows there is a master branch. There are two separate branches called “small feature” and “large feature.” Once you are finished working with the two separate branches, you can merge them and create a master branch.


## Commands List
These are common Git commands used in various situations:

- start a working area (see also: git help tutorial)
   - clone     Clone a repository into a new directory
   - init      Create an empty Git repository or reinitialize an existing one

- work on the current change (see also: git help everyday)
   - add       Add file contents to the index
   - mv        Move or rename a file, a directory, or a symlink
   - restore   Restore working tree files
   - rm        Remove files from the working tree and from the index

- examine the history and state (see also: git help revisions)
   - bisect    Use binary search to find the commit that introduced a bug
   - diff      Show changes between commits, commit and working tree, etc
   - grep      Print lines matching a pattern
   - log       Show commit logs
   - show      Show various types of objects
   - status    Show the working tree status

- grow, mark and tweak your common history
   - branch    List, create, or delete branches
   - commit    Record changes to the repository
   - merge     Join two or more development histories together
   - rebase    Reapply commits on top of another base tip
   - reset     Reset current HEAD to the specified state
   - switch    Switch branches
   - tag       Create, list, delete or verify a tag object signed with GPG

- collaborate (see also: git help workflows)
   - fetch     Download objects and refs from another repository
   - pull      Fetch from and integrate with another repository or a local branch
   - push      Update remote refs along with associated objects

------
## Resources 
#### Getting Help
- If you ever need help while using Git, there are three equivalent ways to get the comprehensive manual page (manpage) help for any of the Git commands:
 `$ git help <verb>` | `$ git <verb> --help` | `$ man git-<verb>`






