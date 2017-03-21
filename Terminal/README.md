# Command Line

In the modern world most development is done through the terminal. I'm not 100% sure why. People could easily create apps with interfaces to do all of this. My guess is, that once you get used to it, it's actually easier.

Terminal is a different way to use your computer. Instead of pointing and clicking you type what you want. On mac you have a built in terminal located in `/Applications/Utilities/Terminal.app`. *look up [file paths](), if you don't know what this means. ex . (Folder/Folder/file.txt)*

We won't be using the built in mac terminal, we will start with a better more improved one.

## iTerm2

Download and install iTerm2 here.

<https://www.iterm2.com>

Download and install my default settings here.

## Basic Terminal Hotkeys

to test these just write a line of random text in the terminal and test out each of these key commands.

*   `ctrl + a` -  jump to beginning of the line
*   `ctrl + e` -  jump to end of the line
*   `ctrl + u` -  clear the current line


### Install iterm2 custom settings

I'll upload custom settings shortly...

### Cool iTerm2 shortcuts

*   `cmd+shift+h` - show paste history
*   `cmd+/` - show cursor if you're lost working on multiple panes
*   `cmd+options+e` - search multiple tabs (mac expose style)
*   `cmd+;` - autocomplete type from previous commands
*   `cmd+d` - split window vertical
*   `cmd+shift+d` - split window horizontal

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

Install oh my zsh by entering into terminal:

```
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

Zsh is configured through the .zshrc file

`.zshrc` is the zsh config file. to edit type `zshconfig`


## Default `.zsrch` file

```shell
# If you come from bash you might have to change your $PATH.
export PATH=$HOME/bin:/usr/local/bin:/Users/Brent/Files/Sites/bin:$PATH
export VAGRANT_HOME=/Users/Brent/Documents/Vagrant/vagrant.d

# Path to your oh-my-zsh installation.
export ZSH=/Users/Brent/Documents/Terminal/oh-my-zsh

# Set name of the theme to load. Optionally, if you set this to "random"
# it'll load a random theme each time that oh-my-zsh is loaded.
# See https://github.com/robbyrussell/oh-my-zsh/wiki/Themes
ZSH_THEME="puddletown"

# Uncomment the following line to use hyphen-insensitive completion. Case
# sensitive completion must be off. _ and - will be interchangeable.
HYPHEN_INSENSITIVE="true"

# Uncomment the following line to disable bi-weekly auto-update checks.
DISABLE_AUTO_UPDATE="true"

# Uncomment the following line to enable command auto-correction.
ENABLE_CORRECTION="true"

# Uncomment the following line to display red dots whilst waiting for completion.
COMPLETION_WAITING_DOTS="true"

# Which plugins would you like to load? (plugins can be found in ~/.oh-my-zsh/plugins/*)
plugins=(git osx textmate bower colorize colored-man-pages extract thefuck docker gulp history z zsh-syntax-highlighting)

# ZSH aliases
alias zshconfig='atom ~/.zshrc'
alias ohmyzsh='atom ~/.oh-my-zsh'
alias reload='. ~/.zshrc'
alias update='brew update && npm update -g && apm update && upgrade_oh_my_zsh'

#misc commands
alias l='ls -lG'
alias a='atom'
alias tmm='sudo fs_usage -f -R filesys backupd'
alias wds='webpack-dev-server --progress --colors'
```


## Add syntax Highlighting

Add syntax highlighting to commands you have not send yet with *zsh-syntax-highlighting*. This will allow you to see colored versons of your commands to visually proof them for errors while you type.

```
$ git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

## Oh My ZSH tips and tricks

[oh-my-zsh cheatsheet](https://github.com/robbyrussell/oh-my-zsh/wiki/Cheatsheet)


1.  You don't have to type `cd` to change directories
2.  Just type `..` to go back 1 directory, `...` to go back 2 etc.
3.  Type `reload` to reload the `.zshrc` file
4.  `update` updates Atom/Node/ZSH/Brew in one command

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

## Install first brew package for ZSH

Install **thefuck**. Corrects mistyped terminal commands so that you don't have to type the whole thing over.

```
$ brew install thefuck
```

1.  tap `esc` twice and it will show you corrections.
2.  typing `fuck` will send the corrected commands

Read more about it here: <https://github.com/nvbn/thefuck>

## Basic Terminal Command Reference

Terminal commands like `ls`, `cd` are just programs that just in the terminal. They often don't have a visual interface. But they're apps all the same like the ones you use on your phone.

### RTFM (Read The Fucking Manual)

`man <program name>`
read the manual pages. Hit `q` to escape the manual pages

*These things look fucked up at first, but it's important to learn how to read them. Keep looking at them with any about commands*

### `d`

`d` - Shows the stack of last used directories
`1` - Typing a number (ex. 1,2,3,4,5) goes to that directory

### `ls`

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

### `cd`

*change directory <argument>*

`cd ..`
		navigates up one directory

`cd ../../`
navigates up 2 directories

`cd ../../<filename>`
		navigates up 2 directories and into <filename>

### Making directories and files

`mkdir` -make new directory

`take path/to/directory` - Makes a new directory in the defined path and moves into it

`tab` - Makes a new tab from the current directory

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
	ex. `grep -textsearch <filename>`
	sort through long files or dir for specific word or character

`cat`
	displays the contents of a text file


`find`
    ex. `find ~/ -iname "filename.txt"`
        `find` finds `~/` in location `"filename.txt"` filename
or...
`“*...*”` *wild card* finds a series of characters within other characters

## SSH to a remote computer

`$ ssh name@ipaddress`

### Setting up ssh keys

<https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2>

## Transfer a file with SCP

**local machine**

`$ scp path/file.txt username@hostname:/var/www/file.txt`

```
-P for portnumber
-r copy whole directories
```

**local file and destination file can also be reversed to download**
