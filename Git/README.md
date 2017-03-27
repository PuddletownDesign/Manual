# GIT

<!-- need to update with -->

Git is the flow of a project. It watches everything that changes. You can revert back to any point of changes or manage a large team of programmers and merge all their work together. It can be difficult to understand some of the concepts, stick with it. It's the underlying foundation of how you will work.

## Reference

This is the best place to start. Work through the examples. *Ignore anything mentioning SVN, you can skip over it.*

<https://www.atlassian.com/git>


## Oh my zsh Shortcuts
Once you learn the commands, use these shortcuts:
<https://github.com/robbyrussell/oh-my-zsh/wiki/Cheatsheet#git>


## Notation
 \* =*zsh shortcut*

## Most Common Git Commands

## Basic Workflow

### Create or clone a project (repo)

`git init` inside a new folder to create a repo

or if there's an existing project you'd like to use:

`git clone <repo url>`

### Save a snapshot of a file

`git add <filename>` - add the file to staging for next commit

### Go back to the last `add command`

`git reset <filename>` - removes a file from staging

`git reset` - without the file name will undo all added files.

### Committing a group of changes

when you make a change and a file has reached a point that it would be good to take a snapshot. You can go back to this point with the next command.

`git commit -m "notes on change"` - This creates a snapshot of a specific change that you made. Think of it like:

1.  Fixed or changed the navbar color
2.  Fixed bug with about section image display

### Go Back to last commit

`git checkout -- <file>` - reverts the file back to previous commit
`git reset HEAD --hard` - bring all files back to previous commit and lose all changes.

### Go Back to a specific commit

`git checkout <commit> <filename>` - reverts a specific file
`git checkout <commit>` - reverts the whole working directory



**Be sure to commit changes that are relevent to the commit message change. Assholes put generic messages or group files in illogical ways. Don't be an asshole.**

### Going back to a previous commit

`git checkout -- <filename>`

### Creating branches for changes or fixes

It's best practice to create a branch and then merge it in with the master branch once it's tested and complete.



### Utility Commands

`GIT INIT` 	Creates a new repository
\*`gi`

`GIT INIT --bare` 	Creates a new bare repository. Used as a central repo
\*`gib`

`GIT STATUS`	Inspects the contents of the working directory
\* `gs`

`GIT LOG`		shows a list of all previous commits
\*`gl`

`GIT HELP LOG`/ `MAN GIT LOG`	shows a manual of all commands

### Staging/ Commiting

`GIT ADD`		adds files from the working directory to the staging area
\* `ga`

`GIT COMMIT`	permanently stores changes from the staging area into the repo
\*`gc`

### Branching/ Checking out
`GIT BRANCH`	list all project branches
`GIT BRANCH <branch name>`	creates a new branch
\*`gb`


`GIT BRANCH -d <branch name>`	Deletes branch
\*`gbd`

`GIT BRANCH -D <branch name>`	force deletes branch
\*`gbD`

`GIT CHECKOUT HEAD`     resets to head of branch
`GIT CHECKOUT HEAD <filename>`	discards changes in the working directory
\*`gch`

`GIT CHECKOUT <branch name>` 	used to switch from one branch to another
\*`gcb`

### Pushing/ Pulling / Cloning
`GIT CLONE <repo url>` - Clones the repository locally
\* `gcl`

`GIT PUSH ORIGIN MASTER` pushes new commits back to github
\*`gpush` - Pushes updates from local to the remote

`GIT PULL ORIGIN MASTER` - Pulls the
\*`gpull` - Pulls the remote updates to the repo

### Diffing / Merging
`GIT DIFF` shows the difference between the working directory and the staging area

`GIT MERGE <branch name>`	used to join file changes from one branch to another *must do from MASTER
\*`gm`

### Reverting

`GIT RESET HEAD <filename>` 	unstages file changes in the staging area
\*`grh`

`GIT RESET SHA` used to reset to a previous commit in your history
