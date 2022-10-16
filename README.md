# git-doc
## list of command 
`$ git status`

The main tool you use to determine which files are in which state is the git status command.

` git add <file> ` -that was to begin tracking files in your directory
`git add .`
In order to begin tracking a new file, you use the command git add.

`$ git diff`
To see what you’ve changed but not yet staged, type git diff 

[It’s important to note that git diff by itself doesn’t show all changes made since your last commit — only changes that are still unstaged. If you’ve staged all of your changes, git diff will give you no output.]


=========================
These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone     Clone a repository into a new directory
   init      Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add       Add file contents to the index
   mv        Move or rename a file, a directory, or a symlink
   restore   Restore working tree files
   rm        Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect    Use binary search to find the commit that introduced a bug
   diff      Show changes between commits, commit and working tree, etc
   grep      Print lines matching a pattern
   log       Show commit logs
   show      Show various types of objects
   status    Show the working tree status

grow, mark and tweak your common history
   branch    List, create, or delete branches
   commit    Record changes to the repository
   merge     Join two or more development histories together
   rebase    Reapply commits on top of another base tip
   reset     Reset current HEAD to the specified state
   switch    Switch branches
   tag       Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects
   
   ==================================
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
        
        
