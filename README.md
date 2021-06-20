# git-cheatsheet

### Init
`git init` - Initialize git in the current folder

### Add
`git add <file-name-1> <file-name-2>...<file-name-N>` (separated by whitespace) - Add files to the staging area

`git add .` - Add files to the staging area

### Commit
`git commit <Commit-message>` - Commit the files from the staging area to repository and opens a text editor to enter the commit message. NOTE: if you want to enter a detailed message about the commit then First line is the Summary of the commit message, leave a blank line below it and then in the next line write the details about the commit.

`git commit -m <Commit message>` - Commit the files from the staging area to the repository with a message, also the flag "-m" will not open a text editor and directly commits

### Branches
`git branch` - list all the branches, also highlights the current branch

`git branch <new-branch-name>` - creates a new branch at the head

`git branch <new-branch-name> <branch-name OR commit-name>` - creates a new branch at the listed branch or the commit

### Checkout
`git checkout <branch-name>` - moves head to the selected branch

`git checkout -b <new-branch-name>` = "-b" flag is used here with checkout here, creates a new branch and move the head to the new branch

`git branch -d <branch-name>` - deletes the listed branch - make sure that you are currently not in the branch you're deleting

### Log
`git log` - list the commits

`git log --stat` - shows more information about the commits

`git log --oneline` - shows the information about the commits in a single line including SHA and the commit message

`git log --oneline --decorate --graph --all` - this will list all the commits in all the branches, this is also show a graph about the branches and the commits in each branch

### Show
`git show` - shows detailed information about the latest commit

### Merge
`git merge <branch-name>` - merges the listed branch into the current branch. NOTE: If a merge conflicts arises, edit the file and keep the changes you want, add it staging area and make a commit like any regular commit.

### Pull
`git pull <remote>` - updates the branch that tracks the remote branch and merge the incoming changes

### Fetch
`git fetch <remote>` - updates the branch that tracks the remote branch but it will not merge the incoming changes to the local branch. It can be seen as **safe**  git pull.

`git fetch --all` or `git pull --all` - updates all the branches that track the remote branches but it will not merge the incoming changes to the local branch.
