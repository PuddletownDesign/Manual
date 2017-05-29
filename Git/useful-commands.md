# Most useful git commands

The purpose of git is to track changes in your code so that you can compare, revert and merge them together. The main goal is to keep a clean git history. Here is a guide to do that.

## Notes

Shortcuts (aliases) are after the hyphen in the title. You can download/reference my git aliases here:

<https://raw.githubusercontent.com/PuddletownDesign/Git/mac/.gitconfig>

## Make a new repo  - `g i`

`git init`

## Clone an existing repo  - `g cl`

`git clone <repo>`

## Pull most recent changes from remote repository  - `g pl`

`git pull`

## Stage files that have been added or changed  - `g a <file>`

`git add <file names or *>`

## Unstage a file  - `g re <file>`

`git reset <filename>`

## Unstage all files  - `g unstage`

`git reset HEAD`

## Stop tracking a file with git you added by mistake - `g rmc <file>`

`git rm --cached <file>`

## Revert repo last commit and trash all changes  - `g lastcommit`

`git reset --hard`

## Revert only a file to last commit  - `g of`

`git checkout -- <file name>`

## Revert repo to previous commit and lose last commit  - `g prevcommit`

`git reset HEAD --hard`

## Use a diff tool to see or revert staged changes vs working changes  - `g d`

`git difftool`

## Use a diff tool to see staged vs. last commit  - `g ds`

`git difftool --staged`

## Combine last 5 commits into 1 commit  - `g res HEAD~5`

**Only do this on feature branch commits that exist locally to you. If you have pushed the feature branch already, just do a normal merge. Basically only rebase branches that only you have access to.**

Say you end up making 5 extra commits because you keep noticing small changes after each commit. Smooch them all down into 1 so you don't pollute the timeline.

`git reset --soft HEAD~5`

Then make 1 commit for the last two

`git commit -m "<message>"`

## Rebasing - Base the history of the feature branch (test) to the most recent commit of the master branch - `g rb <main-branch>`

**Only do this on feature branches that exist locally to you. If you have pushed the feature branch already, just do a normal merge. Basically only rebase branches that only you have access to.**

Use this before/instead of merging a feature branch into the directly. It will keep the timeline clean.

Basically if there is a commit to the master **after** you checked out the feature branch, then the timeline will have a bubble when you go to merge it back in. This fixes that problem.

### check out the feature branch `g o test`

`git checkout test`

### change feature branch link to master to the most recent commit - `g rbm`

`git rebase master`

### check out the master branch - `g om`

`git checkout master`

### merge test in with master - `g m test`

`git merge test`

## Github Specific

### Forking

<https://www.youtube.com/watch?v=5oJHRbqEofs>

### Making Pull Requests

<https://www.youtube.com/watch?v=d5wpJ5VimSU>

## Further Reading

-   <http://sweetme.at/2013/09/29/essential-git-commands-cheat-sheet/>
-   <https://github.com/bpassos/git-commands>
