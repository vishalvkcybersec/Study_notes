To change the default password in a Linux system , we use the command `passwd`

To search the location files in a Linux system, we use any three of these commands

1. `find`
	It can search for files and directories with more than just the name.
	Syntax : find filename
	Example : `sudo find / -name sbd*`




1. `locate`
	Inorder to provide a much shorter search time, locate search is a built in database named locate.db rather than the entire hdd itself. This database is automatically updated on a regular basis by the cron scheduler but it can be updated manually with the `updatedb` command.
	
	Syntax : `locate filename`



1. `which`
	The which command searches through directories defined in the path environment variable for a given  file name. This variable contains a listing of directories,  Linux searches when a command is issued without its path. If a match is found , which returns the full path to the file.