# GIT 
 \* =*zsh shortcut*

## Git Commands

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
`GIT BRANCH`	list all of a git project’s branches
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

`GIT MERGE <branch name>`	used to join file changes from one branch to another *must be done from MASTER
\*`gm`

### Reverting

`GIT RESET HEAD <filename>` 	unstages file changes in the staging area
\*`grh`

`GIT RESET SHA`	can be used to reset to a previous commit in your history





 