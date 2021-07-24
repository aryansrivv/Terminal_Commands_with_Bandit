Level 3 ----> Level 4 of the Bandit Game by Overthewire 
Problem Statement : 

<img width="768" alt="Screenshot 2021-07-24 at 3 46 30 PM" src="https://user-images.githubusercontent.com/74819332/126872114-c551c108-a094-411e-a21e-f4522f0c85e8.png">

so logging into the terminal with the command 
`ssh bandit3@bandit.labs.overthewire.org -p 2220`
and the password `UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK`

Now , it says that the file containing the password lies in the directory `inhere`
<img width="679" alt="Screenshot 2021-07-24 at 4 01 37 PM" src="https://user-images.githubusercontent.com/74819332/126872657-15324c96-8703-4ce9-b660-f2e2b4bec334.png">

we are currently in the directory `bandit3` ( using the command `pwd` which prints the current working directory)
using the command `cd` which changes working directory 
`cd inhere`
now doing `ls` in the `inhere` directory leads to nothing , also in the statement it said that the file is hidden . 
now the command `ls -a` prints the hidden files of the directory too . 
using it we get that there are files named `.  ..  .hidden` in the directory 
we dont yet know the full file name so we do `ls -al` which prints the details of each hidden file 
we now know that `.hidden` is the name of the file containing the password 
Now , we can simply access the content of the file using our `cat ./'.hidden'` command

<img width="567" alt="Screenshot 2021-07-24 at 4 07 07 PM" src="https://user-images.githubusercontent.com/74819332/126872700-da69d2f3-2b41-4bce-9f09-d1cb53c0ed5e.png">
Here's the password 
