# **Command Line**

.zshrc is the zsh config file. to edit type `zshconfig`

## shell prompt
`$`
activates shell

## RTFM

`man <program name>` 
read the manual pages
	- hit `q` to escape the manual pages

## ls

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

***(-a, -l, and -t are options)**
`pwd`
	print working directory

## cd 

*change directory <argument>*
	
`cd ..` 
		navigates up one directory
		
`cd ../../`
navigates up 2 directories

`cd ../../<filename>` 
		navigates up 2 directories and into <filename>

## Making directories and files

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

## other navigation ##


`top`
	shows all programs running/ cpu 
	
`q`
	escapes from list

`clear`
	clears screen

`CONTOL + C`
	cancel running command	
	
## finding things ##	

`whereis`
	finds program ex. whereis perl > user/bin/perl

### the Grepping and the Piping
##### the grepping and the piping
`grep`
	ex. `grep -rachel <filename>`
	sort through long files or dir for specific word or character
	
`cat`
	displays the contents of a text file
	

`find`
    ex. `find ~/ -iname "filename.txt"`
        `find` finds `~/` in location `"filename.txt"` filename 
or…
`“*……*”` *wild card* finds a series of characters within other characters 