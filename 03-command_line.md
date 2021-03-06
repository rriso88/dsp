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

* show current working directory path
* $ pwd
* change working directory
* $ cd newdir
* go up one level
* $ cd ..
* creating a directory
* $ mkdir newdirname
* deleting a directory
$ rmdir newdirname
* creating a file using `touch` command
$ touch filename.extension
* deleting a file
$ rm -Rf filename
* renaming a file
$ mv filename.extension newfilename.extension
* listing hidden files
$ defaults write com.apple.finder AppleShowAllFiles YES
  Press return
  Hold the ‘Option/alt’ key, then right click on the Finder icon in the dock and click Relaunch
* copying a file from one directory to another
mv test/testfilenew.txt test2/testfilenew.txt


---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  : short listing
`ls -a`  : list including hidden files
`ls -l`  : long listing
`ls -lh`  : long listing iwth human readable file sizes
`ls -lah`  : unsure
`ls -t`  : displays newest files first. (based on timestamp)
`ls -Glp`  : unsure



---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

* ls -c : displays files by file timestamp
* ls -m : displays the names a comma-separated list
* ls -r : displays files in revers order
* les -R : displays subdirectories as well
* ls -u : displays files by file access time

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

xargs - build and execute command lines from standard input

EXAMPLE:
find /tmp -name core -type f -print | xargs /bin/rm -f

       Find files named core in or below the directory /tmp and delete them.
       Note that this will work incorrectly if there are any filenames
       containing newlines or spaces.

 

