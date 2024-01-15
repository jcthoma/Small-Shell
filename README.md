# Small-Shell

 The shell will have a loop that reads command lines and process them. The prompt for your shell will be
“shell_jr:␣”. The commands your shell must handle are:
1. exit - When the user enters the exit command the shell will stop executing by calling exit() with the
exit code 0. Before executing exit, the shell will print the message “See you”.
2. goodbye - Has the same functionality as exit.
3. cd - This command changes the current directory. You can assume the user will always provide a direc-
tory as an argument. Assume that a directory name does not include whitespace characters.
4. pushd - This command is used to change the current directory to the directory given as the command-
line argument and simultaneously push the current directory onto a stack of directories. Shell Jr can
keep 16 directories on the stack. If the user try to push more than 16, print the message “Directory stack
is full” and the current directory won’t be changed. Assume that a directory name does not include
whitespace characters.
5. dirs - This command will print the directories in the stack.
6. popd - This command is used to retrieve the directory from the top of the stack and change the current
directory to the directory. It will remove top directory from the stack. If the user try to pop a directory
when the stack is empty, print the message “Directory stack is empty” and the current directory won’t
be changed.
7. A command with a maximum of one argument (e.g., wc location.txt). That means your shell should be
able to handle commands like pwd, date or wc location.txt. Note that these are not shell commands but
executable binaries.
