# SHELL SCRIPT

A Shell script is a computer program designed to be run by a Unix shell, a command-line interpreter.The various dialects of shell scripts are considered to be scripting languages.

# Shell Scripting

Usually, shells are interactive, which means they accept commands as input from users and execute them. However, sometimes we want to execute a bunch of commands routinely, so we have to type in all commands each time in the terminal.
As a shell can also take commands as input from file, we can write these commands in a file and can execute them in shell to avoid this repetitive work. These files are called Shell Scripts or Shell Programs. Shell scripts are similar to the batch file in MS-DOS. Each shell script is saved with **`.sh`** file extension e.g., **myscript.sh**.

A shell script has syntax just like any other programming language. If you have any prior experience with any programming language like Python, C/C++ etc. It would be very easy to get started with it.

A shell script comprises the following elements –

•**Shell Keywords** – if, else, break etc.

•**Shell commands** – cd, ls, echo, pwd, touch etc.
Functions

•**Control flow** – if..then..else, case and shell loops etc.


# Need of Shell Scripts

There are many reasons to write shell scripts:

•To avoid repetitive work and automation.

•System admins use shell scripting for routine backups.

•System monitoring.

•Adding new functionality to the shell etc.


# Advantages of shell scripts

•The command and syntax are exactly the same as those directly entered in the command line, so programmers do not need to switch to entirely different syntax.

•Writing shell scripts are much quicker

•Quick start

•Interactive debugging etc.


#  Disadvantages of shell scripts
 
•Prone to costly errors, a single mistake can change the command which might be harmful.

•Slow execution speed

•Design flaws within the language syntax or implementation

•Not well suited for large and complex task

•Provide minimal data structure unlike other scripting languages. etc.

# Basic and Advanced Shell Commands

1. Is -
Displays information about files in the current directory.

2. pwd-
Displays the current working directory.

3. mkdir-
Creates a directory.

4. cd-
To navigate between different folders.

5. rmdir_
Removes empty directories from the directory lists.

6. cp-
Copy files from one directory to another.

7. mv-
Rename and Replace the files

8. rm-
Delete files

9. uname -
Command to get basic information about the OS

10. locate -
Find a file in the database.

11. touch -
Create empty files

# Debugging in Shell Scripts

Debugging is terminology that means the process of identifying errors and possibly resolving them in computer hardware or software. 

•The most basic step while debugging the script is, **“echo”**. You can “echo” the command on which you are using the variables so that you can check in the output section whether it is taking the right values or not.


1.  Using bash options (-x, -n, -v): The following are various options explained -

• **-x** - It helps in tracing command output before executing them, when we run the script using this option we get each line of code traced before it is executed and its respective output printed in the terminal. The following is a simple HelloWorld.sh script and its execution screenshots depict the same.

#! /bin/bash

#print Hello World

echo 'Hello World'

#Listing all components on root

ls /

• **-n** -  It helps in checking the syntax errors if there are any in the shell script prior to executing it. With a boom in the technology of cloud computing, it is essential to know various command-line options to check syntax errors. It is difficult to have GUI (Graphical User Interfaces) or designated IDEs (Integrated Development Environments) on Virtual Machines executing in the cloud.

• **-v**- If there is a need to read the comments and entire script while the script is executing, then -v option helps us achieve this goal. The following example screenshot shows how -v and -x differ from each other and how we can use -v option.


2.  For extensive debugging, we use **“set”** which is Bash’s built-in.

• **set -x**

The most common one is the -x option, it will run the script in debug mode. Set -x shows the command as well as their output on the terminal so that you would know for which command.

• **set -u**

Sometimes you have not provided the variable, yet you have used it somewhere in the script. So, by default bash will ignore the variable that does not exist. 

• **set -e**

Well, bash will throw an error on any wrong command provided on the script, yet it will continue to execute the remaining part of the script. However, we don’t want bash to accumulate the errors instead, it should stop executing the script on the first error, right away.

• **set +e** means to turn off the -e option, and **set -e** means to turn on set -e again.