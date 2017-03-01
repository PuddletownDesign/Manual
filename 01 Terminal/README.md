# Command Line

## Shell prompt
`$` *indicates the shell prompt in writing*

## Shells and configuration

### zsh

The default shell is usually configured to bash. We want to change the default shell to zsh.

To check your current shell:

```
$ echo $SHELL
```

If it is not set to zsh, do so by entering:

```
$ chsh -s /usr/bin/zsh
```

### Oh my zsh

Oh my zsh is a custom configuration to the zsh shell.

Read about oh my zsh here:

<https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH>

Install oh my zsh by entering:

```
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

Zsh is configured through the .zshrc file

`.zshrc` is the zsh config file. to edit type `zshconfig`

## Installing mac terminal package manager

Brew is the best mac terminal package manager. It can be installed by running:

```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
You can read more about it here:
<https://brew.sh>

## Command Reference

### RTFM

`man <program name>`
read the manual pages. Hit `q` to escape the manual pages

### ls

`ls`= list
	lists directories

`ls -a`
lists directories + files starting with a dot (.hidden)

`ls -l`
lists all contents of a directory in long format

`ls -t `
lists and orders files and directories by time last modified

`ls -alt`
combines all above options

\* **(-a, -l, and -t are options)**
`pwd` print working directory

### cd

*change directory <argument>*

`cd ..`
		navigates up one directory

`cd ../../`
navigates up 2 directories

`cd ../../<filename>`
		navigates up 2 directories and into <filename>

### Making directories and files

`mkdir`
make new directory

`touch`
	create new file within directory

`pico`
	enter text edit to create new file from within iTerm

`cp`
	copy

`cp *<name>`
	selects all files in the working directory

`cp *<origin> <destination>`
		copies all files (origin) into another directory (destination)

`mv`
move file (rename)

`mv <file> <directory>`
moves file into directory

`mv <filenameA.txt> <filenameB.txt>`
changes the filename from a to b

`rm`
remove a file

`rm -r`
remove recursive:
removes a directory and all its child directories

`rm -rf`
force recursive removes directory

### Other navigation


`top`
	shows all programs running/ cpu

`q`
	escapes from list

`clear`
	clears screen

`CONTOL + C`
	cancel running command

### Finding things

`whereis`
	finds program ex. whereis perl > user/bin/perl

### The Grepping and the Piping
`grep`
	ex. `grep -rachel <filename>`
	sort through long files or dir for specific word or character

`cat`
	displays the contents of a text file


`find`
    ex. `find ~/ -iname "filename.txt"`
        `find` finds `~/` in location `"filename.txt"` filename
or...
`“*...*”` *wild card* finds a series of characters within other characters
