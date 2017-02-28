COMMAND LINE

.zshrc is the zsh config file. to edit type zshconfig

$= shell prompt

man <program name> = read the manual pages
	- hit q to escape the manual pages

ls= list  
	lists directories

	ls -a
		lists directories + files starting with a dot (.hidden)
	ls -l 
		lists all contents of a directory in long format
	ls -t 
		lists and orders files and directories by time last modified 
	ls -alt 
		combines all above options

			*(-a, -l, and -t are options)
pwd=
	print working directory

cd= 
	change directory <argument>
	
	cd .. 
		navigates up one directory
	cd ../../
		navigates up 2 directories
	cd ../../<filename> 
		navigates up 2 directories and into <filename>

	

mkdir=
	make new directory

touch=
	create new file within directory

cp= 
	copy

	cp *<name>
		* selects all files in the working directory
	cp *<origin> <destination>
		copies all files (origin) into another directory (destination)

mv= move file (rename)

	mv <file> <directory>/ moves file into directory
	mv <filenameA.txt> <filenameB.txt>  changes the filename from a to b

rm= remove a file
rm -r= remove recursive 
	removes a directory and all its child directories
rm -rf = force recursive removes directory


top=
	shows all programs running/ cpu 
q=
	escapes from list

clear=
	clears screen

whereis= 
	finds program ex. whereis perl > user/bin/perl
grep=
	grep -rachel <filename>
	sort through long files or dir for specific word or character
cat=
	displays the contents of a text file
pico=
	enter text edit to create new file from within iTerm

CONTOL + C=
	cancel running command

find=
find ~/ -iname "neruda.txt"
[command] find
[~/] in location 
[-iname] in name 
[“………..”] file name
or…
[“*……*”] *wild card* finds a series of characters within other characters 