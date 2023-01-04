# Simple Shell
----

## What is Simple shell?

This is a simple implementation of  command-line interpreter for the Unix operating system. 


----
## Learning objetives
* Who designed and implemented the original Unix operating system.
* Who wrote the first version of the **UNIX** shell
* Who invented the B programming language (the direct predecessor to the C programming language).
* Who is Ken Thompson?
* How does a shell work .
* What is a **pid** and a **ppid**.
* How to manipulate the environment of the current process.
* What is the difference between a function and a system call.
* How to create processes.
* What are the three prototypes of main.
* How does the shell use the **PATH** to find the programs.
* How to execute another program with the execve system call.
* How to suspend the execution of a process until one of its children terminates.
* What is **EOF** / “end-of-file”?

----
## Requirements

* All your files will be compiled on **Ubuntu 20.04 LTS** using **gcc 4.8.4** using the flags *-Wall -Werror -Wextra and -pedantic -std=gnu89*.
* All your files should end with a new line.
* Your code should use the [Betty style]
* No more than 5 functions per file.
* All your header files should be include guarded.
* Use system calls only when you need to.

----
## Files incluided in this repository
File |  Description
------------ | -------------
README.md | README file
alias_builtins.c | 
builtin.c | 
builtins_help_1.c | 
builtins_help_2.c | 
env_builtins.c | 
environ.c | 
err_msgs1.c | 
err_msgs2.c | 
errors.c | 
getline.c | 
helper.c | 
helpers_2.c
input_helpers.c | 
linkedlist.c | 
locate.c | 
main.c | 
man_1_simple_shell | manpage
proc_file_comm.c | 
shell.h | Header file
split.c | 
str_funcs1.c | Function that returns a number that coincides two strings
str_funcs2.c | 

----
## Quick start

### Basic Installation
simple_shell is installed by running the following commands in your terminal.

    git clone https://github.com/kanmbieydebra/simple_shell.git

After that simple_shell can compile using

    gcc -Wall -Werror -Wextra -pedantic *.c -o simple_shell

To start, write the following:

    ./simple_shell

----
## Basic operation
When the shell reads the entry, it proceeds through a sequence of operations.

    ls -la

In general terms, the shell reads your entry and divides it into words and operators

ls | -la
------------ | -------------

The shell then analyzes these tokens in commands and other constructs, redirects the input and output as needed, executes the specified command, waits for the output state of the command, and makes that output status available. for further inspection or processing.

----
## Builtin functions
Function | Description | Usage
------------ | ------------- | -------------
env | Show the environment variables |     To show the environment variables

----
## Examples
### Interactive Mode

    $ cat test_ls_2
    /bin/ls
    /bin/ls

### Non-Interactive Mode

    $ cat test_ls_2 | ./hsh
    hsh main.c shell.c test_ls_2

----
## Contributors
* [Adepeju Adekanmbi](https://github.com/kanmbieydebra/simple_shell)
