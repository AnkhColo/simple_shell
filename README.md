Simple shell project by Colin Muriithi and Wamuyu Kamau

The objective of this project is to create a simple shell.

A shell is a command-line interpreter that allows the user
to interact with the operating system by giving commands
and receiving outputs.
It is a user interface that gives access to the underlying operating system
and its features.
It is a program that executes other programs,and it is typically run on
a text-based window.

There are several key components to consider when building a simple shell:

1.Reading user input: 
The shell should continuously read a command from the user and execute it. 
You can use the readline function to read a line of input from the user.

2.Parsing the command: 
The shell should parse the command to extract the command name and any arguments. 
You can use the strtok function to split the input string into tokens.

3.Creating a new process: 
The shell should use the fork function to create a new process and execute the command.

4.Executing the command: 
In the child process, the shell should use the execvp function to execute the command.
The execvp function searches for the specified command in the directories specified in the PATH environment variable.

5.Waiting for the child process to finish: 
In the parent process,
the shell should use the wait function to wait for the child process to finish.

6.Handling errors: 
The shell should handle errors that may occur during the execution of a command,
such as a command not being found or insufficient permissions.

7.Implementing shell built-in commands: 
The shell should support built-in commands such as cd for changing
the current working directory and exit for exiting the shell.

8.Implementing shell scripting:
The shell should allow users to write shell scripts,
which are text files that contain a series of commands to be executed by the shell.

These are the main components to consider when building a simple shell.

