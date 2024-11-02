Custom Unix Shell (lsh)

A Unix-like shell with support for job control, command history, input/output redirection, aliasing, and a set of built-in commands. The lsh shell allows users to interact with the Unix environment in a simplified way, with familiar features found in standard shells.

Project Structure

The code is organized into multiple files, each focusing on specific functionalities:

main.c: The main entry point for the shell, which handles the initialization and command loop.
builtin.c and builtin.h: Contains implementations for built-in commands.
parser.c and parser.h: Responsible for parsing user input.
job_control.c and job_control.h: Manages job control functionalities like jobs, fg, and bg.
execution.c and execution.h: Handles command execution, including piping and redirection.

COMPILATION

readline library: Install this library for command history. To install on Debian-based systems:
-sudo apt-get install libreadline-dev-

"make all"

TO Run: 
"./lsh-"



Built-in Commands

cd - Change the current directory.
help - Display help information for lsh.
exit - Exit the shell.
alias - Create or display command aliases.
unalias - Remove an existing alias.
jobs - List all current background jobs.
fg - Bring a background job to the foreground.
bg - Resume a stopped job in the background.
clear - Clear the terminal screen.
pwd - Display the current working directory.


Job Control

Execute processes in the background using &.
Navigate through command history using up/down arrow keys.
Powered by readline for smooth input handling.


Aliases

Set and view command aliases.
Remove aliases with unalias.


Input/Output Redirection

Use > for output redirection and < for input redirection.
Support for command piping (|) to combine commands.
