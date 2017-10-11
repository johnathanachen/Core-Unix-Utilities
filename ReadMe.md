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
    - `Hello world`
1.  Print a variable value, like `$USER` or `$PATH`
    - `printf $USER`
1.  Set a variable `NAME` equal to your first name, then print its value
    - `set NAME=Johnathan; echo $NAME` not
1.  Set a variable `FULL_NAME` equal to your full name, then print its value
    -  `set FULL_NAME=Johnathan_Chen; echo $FULL_NAME`
1.  Print all environment variables (names and values)
    -  `set`
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

## Challenges, Part 2

These challenges utilize more sophisticated Unix utilities.
Challenges within each section are meant to be solved in order.

### Streams

1.  Print a sentence like `Hello world` into a file named `test.txt`
1.  Append another sentence `Hola Mundo` on a new line of `test.txt`
1.  Print the contents of the file `test.txt`
1.  Print the contents of the file `numbers.txt`
1.  Print the first 10 lines in the file `numbers.txt`
1.  Print the first 5 lines in the file `numbers.txt`
1.  Print the last 10 lines in the file `numbers.txt`
1.  Print the last 5 lines in the file `numbers.txt`
1.  Print lines 6 through 10 in the file `numbers.txt`
1.  Sort all lines in the file `numbers.txt`
1.  Print the first 2 characters of each line in `numbers.txt`
1.  Print only characters 9-16 of each line in `numbers.txt`
1.  Sort the first 2 characters of each line in `numbers.txt`
1.  Print only the unique first 2 characters of each line in `numbers.txt`
1.  Replace all `o`s with `0`s in file `test.txt`
1.  Capitalize all letters in the file `test.txt`
1.  Capitalize all letters in the string `Hello world`

### Search

1.  Find the file named `Cats.txt` in the directory `Animals`
1.  Find all files ending with `.py` in your code directory
1.  Find all files larger than 100 MB in your movies directory
1.  Find all lines containing the word `one` in the file `numbers.txt`
1.  Find all lines containing the letter `e` at least 3 times in the file `numbers.txt`
1.  Find the `search` function definition in a source code file
1.  Find the `search` function definition in all source code files
1.  Count the lines and words in all source code files
1.  Find all U.S. zip codes in a file containing addresses
1.  Find all U.S. zip codes in a file containing addresses
