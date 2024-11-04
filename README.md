# Shell-scripting-notes

## 1. Introduction to Shell Scripting
What is a Shell Script?

A shell script is a text file with a series of commands that a shell (like bash, zsh, sh) can execute. It's commonly used to automate tasks, run batch jobs, and manage system processes.
Why Use Shell Scripting?

Shell scripting is powerful for:

    Automating repetitive tasks
    Scheduling backups
    Managing system configurations
    Processing text files

## 2. Basic Shell Script Structure
#### The Shebang (#!)

    The shebang line at the beginning of a script specifies the interpreter to use.
    Example: #!/bin/bash tells the system to use the bash interpreter.

#### Creating and Running a Script

    Create a Script:
        Open a text editor and add commands. Save it with a .sh extension.

        bash

    nano script.sh

#### Make Executable:

    Make the script executable with chmod.

    bash

    chmod +x script.sh

#### Run the Script:

    Run it by specifying the path.

    bash

        ./script.sh


## 3. Variables
#### Declaring Variables

    Assign variables without spaces around the = sign.

    bash

    NAME="Alice"
    AGE=25

#### Using Variables

    Access variables by prefixing them with $.

    bash

    echo "Name: $NAME, Age: $AGE"

#### Read-Only Variables

    Use readonly to make a variable immutable.

    bash

    readonly PI=3.14

#### Environment Variables

    export a variable to make it available to child processes.

    bash

    export PATH="/usr/local/bin:$PATH"

#### User Input

    Use read to capture input.

    bash

    echo "Enter your name:"
    read NAME
    echo "Hello, $NAME!"


## Operators
### 1. Arithmetic Operators

Arithmetic operators are used to perform mathematical calculations. In shell scripting, arithmetic is often done within $(( ... )) or expr syntax.
Arithmetic Operators
Operator	Description	           Example
+	         Addition	        echo $((5 + 3))
-	        Subtraction	        echo $((5 - 3))
*	        Multiplication	    echo $((5 * 3))
/	          Division	        echo $((5 / 3))
%	      Modulus (remainder)	echo $((5 % 3))
**	        Exponentiation	    echo $((5 ** 2))

#### Examples

bash
A=10
B=5
echo "Addition: $((A + B))"
echo "Subtraction: $((A - B))"
echo "Multiplication: $((A * B))"
echo "Division: $((A / B))"
echo "Modulus: $((A % B))"







  

    
