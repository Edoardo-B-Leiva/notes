[Edoardo Borgia Leiva](https://edoardo-b-leiva.github.io)
# Shell Scripting
Shell scripts are a way to automatize tasks by putting different shell instruction in a file that will be executed sequentially.
Shell scripts end with either `.sh` or `.bash`(not recommended).

## SHABANG!
The first thing to put in a shell script file in general is the "SHABANG" which is the instruction that tells the system which shell to run the script on.

**Examples:**
```Shell
#!/bin/bash #!!MOST COMMON!!
#!/bin/sh
#!/bin/zsh
#!/bin/python
```
## Echo (echo echo echo)
The first thing everyone does when learning a programming language (or similar) is to print "Hello world!" on screen.
In shell scripting you do that by using the `echo` command.

**Example:**
```Bash
#!/bin/bash

echo "Hello world!"
```
## Math Operators
In shell scripts it's possible to make arithmetical operations using the operators below:
```Bash
10+24   #Sum, will give 34
85-42   #Subtraction, will return 43
8*2     #Multiplication, will return 16
2**5    #Power, will return 32
3%2     #Module, will return 1
```
## Variables
Variables are a staple concept in programming and is one of the first thing you will learn in any language
In shell scripting, variables are defined using: `X=<valor>`
## Read, read more...
To get user input 