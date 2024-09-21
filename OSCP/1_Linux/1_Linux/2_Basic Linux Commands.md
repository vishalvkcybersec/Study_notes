`man`
Most linux command line executable programs provide a formal piece of documentation called manual or man pages

Syntax : man command

man -k command is used to do a keyword search

`apropos`
With the apropos command we can search the list of man page descriptions for a possible match based on a keyword.

Both man -k command and apropos command have the same function.


`ls`(Listing Files)
The ls commands prints a basic file listing to the screen. We can modify the output with various wildcards

-a option is used to print all the files including the hidden files
-1 option displays all the files in a single line.

`cd` command
The cd command(change directory) is used to navigate within a Linux system. This command moves to the directory which is specified along with the command.

Syntax : `cd file_path`

`cd ~`   or   `cd`    This goes to the home directory
`cd /`    This goes to the root directory
`cd ..`     This goes to the just one step above the current directory
`cd ../../`   This goes to two steps above the current directory
`cd ../../../`  This goes to three steps above the current directory

`pwd` command
This command is used to print the current  working directories.

`mkdir` command
This command is used to create a directory

Syntax : `mkdir directory_name`

To create multiple directories along with the main directory, we use -p

`mkdir -p test/{recon,exploit,report}`

This command creates a directory with the name test containing three sub directories with the name recon,exploit and report.