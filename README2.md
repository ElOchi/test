# Simple Shell
Shell is a program written by Ken Thompson in 1971, that takes the command inputs written from the the user’s keyboard and passes them to the machine to execute them through the kernel. It also verifies if the command inputs from the user are correct.

## Getting Started

* [Ubuntu 14.04 LTS](http://releases.ubuntu.com/14.04/) - Operating system reqd.

* [GCC 4.8.4](https://gcc.gnu.org/gcc-4.8/) - Compiler used

## Installation
Clone the repository into a new directory
```bash
git clone https://github.com/csoriano2832/simple_shell.git
```
Compile:
```bash
gcc -Wall -Werror -Wextra -pedantic *.c -o shell
```
Execute: 
```bash
./shell
```
or in non-interactive mode:
```bash
echo "ls" | ./shell
```
## Example of Use (FIX IT)
```bash
vagrant@vagrant-ubuntu-trusty-64:~/simple_shell$ ./hsh
($) ls -l
total 72
-rw-rw-r-- 1 vagrant vagrant  1054 Nov 26 01:42 builtin_commands.c
drwxrwxr-x 3 vagrant vagrant  4096 Nov 26 01:42 concepts
-rw-rw-r-- 1 vagrant vagrant   890 Nov 26 01:42 counters.c
-rw-rw-r-- 1 vagrant vagrant  1940 Nov 26 01:42 exec.c
-rw-rw-r-- 1 vagrant vagrant   372 Nov 26 01:42 frees.c
-rwxrwxr-x 1 vagrant vagrant 23170 Nov 26 01:43 hsh
-rw-rw-r-- 1 vagrant vagrant   876 Nov 26 01:42 main.c
-rw-rw-r-- 1 vagrant vagrant   812 Nov 26 01:41 README.md
-rw-rw-r-- 1 vagrant vagrant   304 Nov 26 01:42 remove_new_line.c
-rw-rw-r-- 1 vagrant vagrant   786 Nov 26 01:42 shell.h
-rw-rw-r-- 1 vagrant vagrant   253 Nov 26 01:42 signal_handler.c
-rw-rw-r-- 1 vagrant vagrant   606 Nov 26 01:42 tokenize.c
-rw-rw-r-- 1 vagrant vagrant  1041 Nov 26 01:42 utilities.c
($)
```

### Files  (FIX IT)

| File Name | Description |
| ------ | ------ |
| main.c | Executes programs, verify the locations and handles all functions. |
| string.c | Functions for string manipulation:
|_strcat  _strlen _strcmp | (Concatenates two strings) (Counts the length of a string) (Compares two strings) |
| _getenv.c |Function to gets an environment variable |
| _open_help.c |Function to print env and help |
| builtin_commands.c | Handle all built-ins |
| counters.c | function to count delims of string |
| exec.c | Executes programs, verify the locations and handles all functions |
| frees.c | functions to free memory |
| utilities.c | Contain 5 functions: _strcat (Concatenates two strings),  _strlen (Counts the length of a string), _strcmp (Compares two strings), _strdup (Duplicate a string), _atoi (Convert a string to an integer). |
| more_utilities.c | 2 more functions: _putchar ()writes the character c to stdout), _puts (Prints a string) |
| remove_new_line.c | function to remove a new line char from string |
| shell.h | Libraries and prototypes of functions |
| signal_handler.c | handle the Ctrl + C |
| tokenize.c | function to extract tokens from string |


