# Some Terminal Commands 

## `pwd` - prints out the current working directory 
## `cd` - changes the current working directory to a certain directory.
   `cd /` - changes the directory to the home directory <br/>
   `cd -` - navigates one directory down <br/>
   `cd ..` - navigates one directory up <br/>
   `cd dir1/dir2` to navitage through multiple directories. <br/>
   
## `ls` - prints the contents of the mentioned directory
   `ls dir1` prints the contents of `dir1` ( but it should be in the current directory ) <br/>
   `ls -l` prints the directories and files with some information as well , like owner , type of file , size , date and time last modified etc. <br/>
   `ls -a` Lists out all files including the hidden files , which start out with a `.`  <br/>
   `ls -al` Lists out hidden files along with their information. <br/>
   `ls -lh` lists out all the files in human readable format 
   
## `mkdir dir1` - creates a new directory with name `dir1`

## `file ./*` OR `file *`- lists out the type of every file in the directory <br/>
   `file ./dir*` - lists out the type of every file within the directory which contains the name `dir` <br/>
   `file -b ./*` - lists out types in brief mode <br/>
   
## `find` Command - Searches for a specific or a set of files in a directory or it's hierarchy
   `.` OR `./` - Current working directory <br/>
   `/` - Root directory <br/>
   `-type f` - type of file <br/>
   `-readable` - matches readable files <br/>
   `-executable` - looks for files which are executable and directories which are searchable <br/>
   `-size 1033c` - file uses `1033` units of space , here `c` is for bytes . <br/>
   `-user ABC` - file is owned by user `ABC` <br/>
   `-group XYZ` - file belongs to group `XYZ` <br/>
   `2>/dev/null` - removes the permission denied type of files <br/>
   
## `grep` - Used to look for specific word or pattern in a file 
   ### format --> `grep [options] pattern [files]` <br/>
   ### options
   -c : prints the count of the lines that match a pattern <br/>
   -l : displays list of filename only <br/>
   -n : display matched lines and their line numbers <br/>
   -v : prints all those lines which do not match the pattern <br/>
   -i : Case sensitive search <br/>
   -w : matches whole word <br/>
   -e : to look for multiple patterns <br/>
   -A n : prints searched lines and n lines after the result <br/>
   -B n : prints searched lines and n lines before the result <br/>
   -C n : prints searched lines and n lines after and before the result <br/>
   
   e.g :::: `grep -l "ARYAN" *` will look for "ARYAN" in every file of that dir <br/>
       :::: `grep "^ARYAN" file.txt` will look for lines only that start with "ARYAN" in file.txt(to look for lines that end with it use "ARYAN$" )<br/>
       :::: `grep -e "AR" -e "ARY" -e "ARYA" f1.txt f2.txt` <br/>
       
