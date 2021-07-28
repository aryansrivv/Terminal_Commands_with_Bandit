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
   
