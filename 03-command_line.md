# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

`pwd` = show current working directory path
`mkdir <name>` = create a directory
`rm -rf <name>` = delete a directory, including its contents
`touch <name>` = create file
`rm <name>` = delete file
`mv <name> <new path/name>` = rename or move file
`cp <name> <target>` = copy file to <target>. If the target is a directory, the file will be copied into the directory. Otherwise, the copy is created with the <target> as its name.
`ls -la` = list all files including hidden files
`ls -ld .?*` = list only hidden directories
`chmod` = change permissions of file
`grep -r <keyword> <target>` = recursively search <target> contents, including files and subdirectories, for <keyword>
`df -h` = check disk space used, results in human readable format

---

### Q2.  List Files in Unix   

What do the following commands do:
`ls` = list files by name
`ls -a` = list all files
`ls -l` = list files in long format including permissions, size, timestamp, etc.
`ls -lh` = list files in long format but with size in bytes (human readable)
`ls -lah` = list all files in long format with size in bytes
`ls -t` = list files by most recently modified, then by lexicographical order
`ls -Glp` = list files in long format with '/' appended to directories (not sure what -G does)

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

`ls -L` = symlink
`ls -R` = display subdirectories
`ls -1` = 1 file per line
`ls -u` = list files by most recently accessed
`ls -S` = list files by size, largest first

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

xargs reads data from standard input and performs the specified command (or echo by default if command is not specified) on each item of the input, treating blanks and spaces as delimiters.

Example: I want to delete all files in my current directory with "test" in the filename. The first command lists the files that match and the second part runs 'rm' on each of the files.

find ./ -name '*test*' | xargs rm



 

