## Level 4 ----> Level5

Problem Statement <br/>

<img width="958" alt="Screenshot 2021-07-25 at 2 35 11 PM" src="https://user-images.githubusercontent.com/74819332/126901330-dd56f893-8170-46e3-bd26-4fd1f79191ee.png">

Now logging into the server with the following username and password : 
ssh `bandit4@bandit.labs.overthewire.org -p 2220` and password `pIwrPrtPN36QITSp3EQaw936yaFoFgAB`


The question says that the password is in the "ONLY HUMAN READABLE FORMAT" in the `inhere` directory . <br/> 

Heading towards the `inhere` directory and looking up the files in there we get that there are 9 files with names `-file0*` 
where * goes from 0 to 9 <br/>

<img width="569" alt="Screenshot 2021-07-25 at 2 38 12 PM" src="https://user-images.githubusercontent.com/74819332/126901479-73ee3323-1cc3-479f-a28b-fac318eae350.png">

You will see that `ls -lh` won't work here as it will give all the files present there 

### The `file` Command 
You can use this command to determine the type of a particular file <br/>
since here there are many files we can simply use `file ./*` to determine type of every file <br/>
here `*` is used to list out every possible preceeding `*` <br/>
alternatively , since each of the file have common names upto `-file0` you can also use : <br/>
`file ./-*` OR `file ./-f*` OR `file ./-fi*` OR upto `file ./-file0*` <br/>
remember all these commands will give same result as they all list out all the files <br/>

<img width="733" alt="Screenshot 2021-07-25 at 2 42 56 PM" src="https://user-images.githubusercontent.com/74819332/126901869-8537e9a3-b0b3-41cb-87a7-29fd8755e75c.png">

You can see that `-file07` is in ASCII format which is human readable <br/>
using the command `cat ./"-file07"` we get our password <br/>
