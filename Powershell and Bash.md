# POWERSHELL

• PowerShell is a tool that allows IT professionals to interact with a command-line interface and automate tasks. It can also function as a scripting language.

• PowerShell is a Microsoft tool that provides programming features for automation, configuration management, and scripting. PowerShell is also an open-source command-line interface compatible with Windows, macOS, and Linux. You can use PowerShell in a number of different ways to help programmers save time on repetitive or time-consuming tasks. 

• It  is designed especially for the system administrators. Its analogue in Linux OS is called as a Bash scripting. Unlike other shells, which accepts and return text, it is built on the top of the **.NET** framework, CLR (Common Language Runtime) and DLR (Dynamic Language Runtime). So, it can accept and returns .NET Framework objects.


# Use Of Powershell

• It is both a scripting language and a command-line Shell.

• It can interact with a different number of technologies.

• Windows PowerShell allows complete access to all the types in the .NET framework.

• PowerShell is object-based.

• Many interfaces of GUI that Microsoft designed for its various products are front end interfaces to PowerShell.

• It is more secure than running VBScript or other scripting languages.

• It allows performing repetitive tasks more efficiently by combining multiple commands and by writing scripts. Suppose, a system administrator wants to create hundreds of active directory users, he can achieve this with the help of only some PowerShell cmdlets placed in a script.

• Many complex and time-consuming configurations and tasks can be done in a second with simple cmdlets of PowerShell.


# Advantages of PowerShell


• It is easy to learn and implement.

• It is an object-based scripting language.

• It provides more functions as compared to VBScript and cmd.exe

• PowerShell supports automation platform, which is also an important factor.

• We can also execute a .NET code in PowerShell.
In PowerShell, there is no need to specify the "type" of a variable.

• It is also interactive. It allows programmers to try first at a console and then work with more complicated scripts.

• There is a concept of background jobs in PowerShell scripting.


# Disadvantages of PowerShell

• **Framework** - It requires .NET framework.

 • **Object-based** - With most shells, the text-based commands are used to get the work done while writing scripts. If a user switches to Windows PowerShell from some other type of shells, he will have to get used to a different way of thinking. Due to this, some users need more time to understand the PowerShell.

• **Security risks** - Another drawback of using PowerShell is that it can create some potential security risks. Many professionals of IT use it as a way to connect remotely to other servers and computers. During this process, PowerShell can leave some holes open for security breaches. It is the major disadvantages of using PowerShell script.

• **Web Server** -  Another drawback of PowerShell is that it requires a user to run a web server on his server when utilizing remote functionality.


# Bash ( Bourne Again Shell)

Bash is a shell program written by Brian Fox as an upgraded version of Bourne Shell program 'sh'. It is an open source GNU project. It was released in 1989 as one of the most popular shell distribution of GNU/Linux operating systems. It provides functional improvements over Bourne Shell for both programming and interactive uses. It includes command line editing, key bindings, command history with unlimited size, etc.

• Bash is a command line interpreter that typically runs in a text window where user can interpret commands to carry out various actions. The combination of these commands as a series within a file is known as a Shell Script. Bash can read and execute the commands from a Shell Script.

# Features of Bash

• Bash is sh-compatible as it derived from the original UNIX Bourne Shell. It is incorporated with the best and useful features of the Korn and C shell like directory manipulation, job control, aliases, etc.

• Bash can be invoked by single-character command line options as well as by multi-character command line options also like --debugger, --help, --login, etc.

• Bash Start-up files are the scripts that Bash reads and executes when it starts. Each file has its specific use, and the collection of these files is used to help create an environment.

• Bash consists of Key bindings by which one can set up customized editing key sequences.

• Bash contains one-dimensional arrays using which you can easily reference and manipulate the lists of data.

Bash comprised of Control Structures like the select construct that specially used for menu generation.

# Applications of Bash Scripts

• Manipulating files

• Executing routine tasks like Backup operation.

• Automation


# Advantages of Bash Scripts

• It is simple

• It helps to avoid doing repetitive tasks

• Easy to use

• Frequently performed tasks can be automated

• A sequence of commands can be run as a single command


# Disadvantages of Bash Scripts

• Any mistake while writing can be costly.

• A new process launched for almost every shell command executed

• Slow execution speed 

• Compatibility problems between different platforms

# How to Write Bash Scripts?

• To write a Bash Script  –

• First, we will create a file with the .sh extension.

• Next, we will write down the bash scripts within it.

• After that, we will provide execution permission to it.

• To create and write a file with the .sh extension we can use gedit text editor. The command for it will be –

**gedit scriptname.sh** - 
The first line of our script file will be –

**#!/bin/bash**  - 
This will tell, the system to use Bash for execution. Then we can write our own scripts.