
Bash maintains a record of commands that have been entered into the shell
This can be displayed with the `history` command.

Rather than retyping a long command from the history, we can make use of the history expansion facilities.

Each entry in our history is preceded by a line no.
To rerun a command, we simply type in the exclamation sign followed by the line no

!32

This runs the command saved in line 32 in the the command history.

The double exclamation mark (`!!`) which repeats the last command that was executed during our terminal session.

The command history file is stored in the .bash_history in the users home directory.

Two env variables control the history size  , $HISTSIZE  and $HISTFILESIZE

$HISTSIZE  -  It controls the no of commands the no of commands stored in memory for the the current session.

$HISTFILESIZE  -  It configures how many commands are kept in the history files.

These variables can be edited according to our needs and  saved to the bash configuration files  .bash_history

The up and down arrow can be used to browse through the history within the terminal

Holding CTRL + R will invoke the reverse i search facility.
This can be used to search the command from the hsitory.