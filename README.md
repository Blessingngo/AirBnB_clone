# 0x00. AirBnB clone - The console

## Description

This is a project to build a clone of [AirBnB] (https://www.airbnb.com/).
The console is a command interpreter to help manage objects abstraction and how they are stored.

The console will perform the following tasks:
0. user authentication and authorization
1. create a new object
2. retrieve an object from a file
3. do operations on objects
4. destroy an object

## How to start

## Installing
Clone the repository of the project from GitHub

git clone https://github.com/Blessingngo/AirBnB_clone.git

After doing this, you will have a folder called AirBnB_clone. To help the program work, there will be several files.

/console.py
models/engine/file_storage.py
models/_init_.py
models/base_model.py
models/user.py
models/state.py
models/city.py
models/amenity.py
models/place.py
models/review.py

## How to use it

You can use it both in interactive and non-interactive mode

In Interactive mode, the console will display a prompt (hbnb) showing that the user can write and execute a command. After which the command is run and the prompt will appear again and wait for a new command. This will go on indefinitely as till the user exit the program.

$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$

In Non-interactive mode, the shell will need to be run with a command input piped into its execution to enable the command runs as soon as the Shell starts. In this mode no prompt will appear, and no further input will be expected from the user.

$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$


## Description of the command Input

To give commands to the console, these will need to be piped through an echo in case of Non-interactive mode.

But in Interactive Mode, the commands will need to be written with a keyboard when the prompt appears and will be recognized when the enter key is pressed (new line). Once this happens, the console will attempt to execute the command through several means or will show an error message if the command didn't run successfully. In this mode, you can exit the console  using the CTRL + D combination, CTRL + C, or the command quit or EOF.

## Author

Blessing Victor
