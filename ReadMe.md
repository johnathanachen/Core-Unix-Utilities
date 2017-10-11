# Core: Unix Utilities

_More powerful than the spiky blue shell_

## Challenges, Part 1

Challenges within each section are meant to be solved in order.

### Navigation

1.  Print the path of your working directory
    - `pwd`
1.  List the files in your working directory
    - `ls`
    - `ls .`
1.  List the files with a particular extension, like `.txt` 
    - `ls *.txt`
1.  List the files in a subdirectory, like `project`
    - `ls project/`
    - `ls ./project/`
    - `ls */*`
    - `ls **/*`
1.  Navigate to a subdirectory, like `project`
    - `cd project`
    - `cd ./project`
1.  Navigate to the parent directory of your working directory
    - `cd ..`
    - `cd ./..`
1.  Navigate to a nested subdirectory, like `path/to/project`
    - `cd path/to/project`
1.  Navigate to your home directory
    - `cd`
1.  Navigate back to the previous directory
    - `cd -`
### Variables

1.  Print a sentence, like `Hello world`
    - `echo Hello world`
1.  Print a variable value, like `$USER` or `$PATH`
    - `printf $USER`
1.  Set a variable `NAME` equal to your first name, then print its value
    - `set NAME=Johnathan; echo $NAME` not
1.  Set a variable `FULL_NAME` equal to your full name, then print its value
    -  `set FULL_NAME=Johnathan_Chen; echo $FULL_NAME`
1.  Print all environment variables (names and values)
    -  `evn`
    - `printenv`
    - `compgen -v`
1.  Make an alias named `hello` that prints `Hello world`
    - `alias hello='echo "Hello world"'`
1.  Make an alias named `gocode` that navigates to your code directory
    - `alias gocode='cd /Users/Johnathan/Desktop/Makeschool/Core-Unix-Utilities/`
1.  Print all aliases (names and values)
    - `alias`
### Getting Help

1.  Print what options a command accepts, like `bash` or `python`
    - `bash --help`
1.  Read the manual for a command, like `echo` or `ls`
    - `man echo`
1.  Print the file path to a command, like `bash` or `python`
    - `realpath bash`

## Challenges, Part 1

Challenges within each section are meant to be solved in order.

### Navigation

1.  Print the path of your working directory
1.  List the files in your working directory
1.  List the files with a particular extension, like `.txt`
1.  List the files in a subdirectory, like `project`
1.  Navigate to a subdirectory, like `project`
1.  Navigate to the parent directory of your working directory
1.  Navigate to a nested subdirectory, like `path/to/project`
1.  Navigate to your home directory
1.  Navigate back to the previous directory

### Variables

1.  Print a sentence, like `Hello world`
1.  Print a variable value, like `$USER` or `$PATH`
1.  Set a variable `NAME` equal to your first name, then print its value
1.  Set a variable `FULL_NAME` equal to your full name, then print its value
1.  Print all environment variables (names and values)
1.  Make an alias named `hello` that prints `Hello world`
1.  Make an alias named `gocode` that navigates to your code directory
1.  Print all aliases (names and values)

### Files

1.  Navigate to the directory `Animals`
	- `cd Animals`
1.  Print the contents of the file `Cats.txt`
	- `cat Cats.txt`
1.  Print the contents of both files `Cats.txt` and `Dogs.txt`
	- `cat Cats.txt Dogs.txt`
1.  Count the words in the file `Cats.txt`
	- `wc -w Cats.txt`
1.  Count the words in all files with the extension `.txt`
	- `wc -w *.txt`
1.  Copy the file `Dogs.txt` to a new file `BabyDogs.txt`
	- `cp Dogs.txt BabyDogs.txt`
1.  Rename the file `BabyDogs.txt` to `Puppies.txt`
	- `mv BabyDogs.txt Puppies.txt`
1.  Make a new directory named `Shelter` inside `Animals`
	- `mkdir Shelter`
1.  Move the file `Puppies.txt` into the directory `Shelter`
	- `mv Puppies.txt Shelter/Puppies.txt`
1.  Copy the file `Cats.txt` to `Kittens.txt` inside `Shelter`
1.  List the files within the directory `Shelter`
1.  Count the words in all `.txt` files inside `Shelter`
1.  Try to remove the directory `Shelter` (this should fail)
1.  Remove all `.txt` files inside `Shelter`
1.  Remove the directory `Shelter` (this should succeed)
1.  Now cry because you just deleted those poor tiny animals

### Permissions

1.  Print out your user name
1.  List the permissions (and metadata) of all `.txt` files
1.  Give all users write permission on the file `Cats.txt`
1.  List the permissions (and metadata) of the file `Cats.txt`
1.  Change the owner of the file `Cats.txt` to another user
1.  Now list the permissions (and owner) of the file `Cats.txt`
1.  Try to change the owner of the file `Cats.txt` back to yourself
1.  Invoke the super-user to make the previous command succeed
1.  List the permissions (and owner) of the file `Cats.txt` again


## Challenges, Part 2

These challenges utilize more sophisticated Unix utilities.
Challenges within each section are meant to be solved in order.

### Streams

1.  Print a sentence like `Hello world` into a file named `test.txt`
    - `echo "Hello world" > test.txt`
1.  Append another sentence `Hola Mundo` on a new line of `test.txt`
    - `echo "Hola Mundo" >> test.txt` 
1.  Print the contents of the file `test.txt`
    - `cat test.txt`
1.  Print the contents of the file `numbers.txt`
    - `cat Numbers/numbers.txt`
1.  Print the first 10 lines in the file `numbers.txt`
    - `sed -n 1,10p numbers.txt`

1.  Print the first 5 lines in the file `numbers.txt`
    - `sed -n 1,5p  numbers.txt`
1.  Print the last 10 lines in the file `numbers.txt`
    - `tail -10  numbers.txt`
1.  Print the last 5 lines in the file `numbers.txt`
    - `tail -5  numbers.txt`
1.  Print lines 6 through 10 in the file `numbers.txt`
    - `sed -n 6,10p numbers.txt`
1.  Sort all lines in the file `numbers.txt`
    - `sort numbers.txt`
1.  Print the first 2 characters of each line in `numbers.txt`
    - ``
1.  Print only characters 9-16 of each line in `numbers.txt`
    - ``
1.  Sort the first 2 characters of each line in `numbers.txt`
    - ``
1.  Print only the unique first 2 characters of each line in `numbers.txt`
    - ``
1.  Replace all `o`s with `0`s in file `test.txt`
    - ``
1.  Capitalize all letters in the file `test.txt`
    - ``
1.  Capitalize all letters in the string `Hello world`
    - ``
### Search


1.  Find the file named `Cats.txt` in the directory `Animals`
    - ``
1.  Find all files ending with `.py` in your code directory
    - ``
1.  Find all files larger than 100 MB in your movies directory
    - ``
1.  Find all lines containing the word `one` in the file `numbers.txt`
    - ``
1.  Find all lines containing the letter `e` at least 3 times in   the file `numbers.txt`
    - ``
1.  Find the `search` function definition in a source code file
    - ``
1.  Find the `search` function definition in all source code files
    - ``
1.  Count the lines and words in all source code files
    - ``
1.  Find all U.S. zip codes in a file containing addresses
    - ``
1.  Find all U.S. zip codes in a file containing addresses
    - ``