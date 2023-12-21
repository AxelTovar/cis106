---
name: Axel Tovar
course: cis106
semester: Fall 23
---

# Final Assignment

## Question

## Question 1

## awk
* Description:
    * awk is a scripting language use for processing and displaying text.
 * Formula:
 * 'awk + options + {awk command} + file'
 * 'command output' | 'awk + options + {awk command}'
 * Examples:
    * How to print the first field of a file:
      * 'awk -F':' '{print $1}' /etc/passwd'
    * How to start printing form a different line
      * 'awk 'NR > 3 {print}' /etc/passwd'
    * How to change a field to upper case:
      * 'awk -F: '{print toupper($1)}''
## cat
* Description:
    * Used for seeing the content of a file. Also used for concatenating files.
 * Formula:
 * 'car + option + file or files to view/concatinate'
 * Examples:
    * How to see the content of a file:
      * 'cat /etc/passwd'
    * How to see the content of a file with line numbers:
      * 'cat -n /etc/passwd'
    * How to see the content of a file with ending line character
      * 'cat -E /etc/passwd'
## cp
* Description:
    * Used for copying a file.
 * Formula:
 * 'cp + option + file'
 * Examples:
    * How to copy a file
      * 'cp banna.txt ~/Documents'
    * How to copy a directory
      * 'cp -r Documents/Books Downloads/'
    * How to copy all files in a directory
      * 'cp Documents/Books* Downloads/'

## cut
* Description:
    * Used to extract a specific section of each line of a file and display it on the screen.
 * Formula:
 * 'cut + option + file(s)'
 * Examples:
    * How to cut a file excluding a given field
      * 'cut -d ',' --Dracula -s -f3 dracula.txt'
    * How to display a list of all users in your system
      * 'cut -d':' -f1 /etc/passwd'
    * How to cut a range of bytes per line
      * 'cut -b 1-b /etc/passwd'
## grep
* Description:
    * Used to search text in given file. Grep works line by line basis.
 * Formula:
 * 'grep + option + search criteria + file'
 * Examples:
    * How to search any line containing the word love
      * 'grep 'love' ~/Documents/Books/pride-and-prejudice.txt'
    * How to search all lines that don't include 'dracula'
      * 'grep -v 'dracula' ~/Documents/Books/dracula.txt'
    * How to search all line that repeat a certain word 3 times
      * 'grep -E "A{3}" banna.txt'
## head
 Description:
    * Used to displays the top N number of line oof a given file.
 * Formula:
 * 'head + option + file'
 * Examples:
    * How to display the first 5 lines
      * 'head -5 /etc/passwd'
    * How to display the first 10 lines
      * 'head /etc/passwd'
    * How to display the first 50 lines
      * 'head -50 /etc/passwd'
## ls
 Description:
    * Used to list all names of files and directories.
 * Formula:
 * 'ls + option + file or directory
 * Examples:
    * How to list names of files and directories in lowercase
      * 'ls -s ~/Documents'
    * How to list all names of files and directories in a table
      * 'ls -l /etc/passwd'
    * How to list all names of files and directories including hidden files
      * 'ls -a ~/Documents'
## man
 Description:
    * Used to document files.
 * Formula:
 * 'man + option + file'
 * Examples:
    * How to open man page of passwd
      * 'man /etc/passwd'
    * How to show all available pages
      * 'man -a /etc/passwd'
    * How to access the manuel
      * 'man ls'
## mkdir
 Description:
    * is used for creating one or multiple directories.
 * Formula:
 * 'mkdir + name of directory'
 * Examples:
    * How to create a directory in a different directory
      * 'mkdir ~/Pictures/flowers'
    * How to create a directory in your current directory
      * 'mkdir flowers'
    * How to create multiple directories
      * 'mkdir ~/Pictures/flowers ~/Pictures/towns ~/Pictures/landscapes'
## mv
 Description:
    * Used to move and rename files or directories.
 * Formula:
 * 'mv + source + destination'
 * Examples:
    * How to rename a file
      * 'mv banna.txt banana.txt'
    * How to move multiple directories to a different directory
      * 'mv games/ wallpapers/ rockmusic/ /media/student/flashdrive/
    * How to rename a file but keeping the directory the same
      * 'mv banna.txt ~/Pictures/banana.txt'
## tac
 Description:
    * Used for displaying the content of a file in reverse order.
 * Formula:
 * 'tac + option + file(s) to display'
 * Examples:
    * How to display the content
      * 'tac /etc/passwd'
    * How to display the content using absolute path
      * 'tac ~/Documents/Books/dracula.txt'
    * How to attach the separator
      * 'tac -b characters.txt'
## tail
 Description:
    * Used to display the last N number of lines of a given file.
 * Formula:
 * 'tail + option + file'
 * Examples:
    * How to display the last 10 lines of a file
      * 'tail ~/Documents/Books/dracula.txt'
    * How to display the last 20 lines of a file
      * 'tail -5 /etc/passwd'
    * How to display account information of the last user
      * 'tail -1 /etc/passwd'
## touch
 Description:
    * Used for creating files
 * Formula:
 * 'touch + name of file'
 * Examples:
    * How to create several files
      * 'touch names.txt schedule.txt assignments.txt'
    * How to create a file using absolute path
      * 'touch ~/Downloads/tools.txt'
    * How to create a file with space
      * 'touch "list of objects.txt"'
## tr
 Description:
    * Used for translating or deleting characters from standard output.
 * Formula:
 * 'standard output | tr + option + set + set'
 * Examples:
    * How to translate one character to another
      * 'cat banana.txt | tr '.' ','
    * How to translate space to tabs
      * 'cat banana.txt | tr "[:space:]" '\t''
    * How to translate tabs into space
      * 'cat banana.txt | tr -s "[:space:]" ' ''
## tree
 Description:
    * Used to list files and directories.
 * Formula:
 * 'tree + option
 * Examples:
    * How to list directories only
      * 'tree -d ~/Documents'
    * How to sort files alphanumerically
      * 'tree -dv ~/Documents'
    * How to print the date of last modification
      * 'tree -D ~/Documents'

## Question 2
* How to work with multiple terminals open?
  * On the top right of the terminal there are two buttons to press one to split horizontally and one to split vertically.
* How to work with manual pages?
  * Type 'man man' to get a manual page.
* How to parse (search) for specific words in the manual page
  *Type 'man man | grep "option"'. 
* How to redirect output (> and |)
  * 'torch > banna.txt' and 'torch | tree banna.txt'.
* How to append the output of a command to a file
  * 'notes >> characters.txt'
* How to use wildcards
  * For copying and moving multiple files at the same time
    * 'cp Pictures/*.png Pictures/*.jpg Downloads/'
* How to use brace expansion
  * For creating entire directory structures in a single command
    * mkdir -p bigpaperwork/{work1/{paper1,paper2},work2,work3}