# Command Line

In the modern world most development is done through the terminal. I'm not 100% sure why. People could easily create apps with interfaces to do all of this. My guess is, that once you get used to it, it's actually easier.

Terminal is a different way to use your computer. Instead of pointing and clicking you type what you want. On mac you have a built in terminal located in `/Applications/Utilities/Terminal.app`. *look up [file paths](), if you don't know what this means. ex . (Folder/Folder/file.txt)*

We won't be using the built in mac terminal, we will start with a better more improved one.

## iTerm2

Download and install iTerm2 here.

<https://www.iterm2.com>

Download and install my default settings here.

### Install iterm2 custom settings

I'll upload custom settings shortly...

## Shell prompt

The shell prompt is the line of text right before the blinking cursor.

`$` *indicates the shell prompt in writing* - **If you copy and paste, DO NOT copy the dollar sign ($) from the examples. Only the text after it.**

## Shells and configuration

The shell is the program that interprets your input. The default shell is normally configured to bash. We want to change the default shell to zsh.

### zsh (Z shell)

Zsh is more modern and a lot more extensible. We'll still use bash at times, however not for general purposes.

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

#### Read about oh my zsh here:

<https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH>

[oh-my-zsh cheatsheet](https://github.com/robbyrussell/oh-my-zsh/wiki/Cheatsheet)

Install oh my zsh by entering into terminal:

```
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

Zsh is configured through the .zshrc file

`.zshrc` is the zsh config file. to edit type `zshconfig`

## Installing mac terminal package manager

A terminal package manager is like the app store or google play store for terminal. It downloads and installs programs for you to use. Brew is the best mac terminal package manager. It can be installed by running:

```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

To install a program that you don't have simply type:

```
$ brew install <program name>
```

You can read more about it here:

<https://brew.sh>

## Basic Terminal Command Reference

Terminal commands like `ls`, `cd` are just programs that just in the terminal. They often don't have a visual interface. But they're apps all the same like the ones you use on your phone.

### RTFM (Read The Fucking Manual)

`man <program name>`
read the manual pages. Hit `q` to escape the manual pages

*These things look fucked up at first, but it's important to learn how to read them. Keep looking at them with any about commands*

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
