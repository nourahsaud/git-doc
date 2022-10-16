# A Simple Git Explanation

![Git-Logo](https://wac-cdn.atlassian.com/dam/jcr:f6948a92-f446-466f-8783-1dd1cbcc661a/hero.svg?cdnVersion=578)

## What is Git and Why we need it?
Git is a version control system [(VCS)](a "Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.") that developers use all over the world. It helps you track different versions of your code and collaborate with other developers.
Git helps you to track of which changes were made, by whom, and when those changes were made. 


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

## Installing Git
In order to check if you already have Git installed on your computer you can type the command `git --version` in the terminal.

If you already have Git installed then you will see what version you have. If you don’t have Git installed you can visit the [Git website](https://git-scm.com/downloads) and easily follow the download instructions to install the correct version for your operating system.

## Git Basics 

Branch in Git

Branch in Git is used to keep your changes until they are ready. You can do your work on a branch while the main branch (master) remains stable. After you are done with your work, you can merge it with the main office.

The above diagram shows there is a master branch. There are two separate branches called “small feature” and “large feature.” Once you are finished working with the two separate branches, you can merge them and create a master branch.

HEAD -> head 


=================
## Commands list 
## tutorial 
==============================
## Resources 
#### Getting Help
- If you ever need help while using Git, there are three equivalent ways to get the comprehensive manual page (manpage) help for any of the Git commands:
 `$ git help <verb>` | `$ git <verb> --help` | `$ man git-<verb>`





