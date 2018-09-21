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

- **pwd** shows current working directory path. 
- **mkdir** creates a directory. 
- **rm -r** deletes a directory. 
- **touch** creates a file. 
- **rm** deletes a file. 
- **mv** renames a file. 
- **ls -a** lists hidden files. 
- **cp** copies a file from onr directory to another. 
- **cat** shows contents of a file. 
- **sort** sorts lines of text alphabetically. 
- **uniq** filters duplicate, adjacent lines of text. 
- **grep** searches for a text pattern and outputs it. 
- **sed** searches for a text pattern, modifies it, and outputs it. 


---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

- **ls** lists files and directories in the current directory. 
- **ls -a** lists all contents including hidden files and directories. 
- **ls -l** lists contents of a directory in long format. 
- **ls -lh** lists contents of a directory in long format and in human readable size. 
- **ls -lah** lists contents in long format, human readable size including hidden contents. 
- **ls -t** orders files and directories by the time they were last modified. 
- **ls -Glp** enables '-l' option, disables writing the files owner name or number and writes a '/' 
after each file if it is a directory. 

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

- **-d** displays only directories. 
- **-R** displays subdirectories as well. 
- **-u** displays files by the file access time. 
- **-q** displays all nonprinting characters as '?'  
- **-1** displays each entry on a line.  


---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

xargs is a command on Unix and most Unix-like operating systems used to build and execute
commands from standard input. It converts input from standard input into arguments to a command. 
'''
find /path -type f -print | xargs rm.  
'''
In the above example, the '''find''' utility feeds the input of '''xargs''' with a long list of file names. '''xargs''' then
splits this list into sublists and calls '''rm''' once for every sublist.  

 

