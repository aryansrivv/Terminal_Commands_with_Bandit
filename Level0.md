The Level 1 of the game contains the following statement :- 


**The password for the next level is stored in a file called readme located in the home directory.**
**Use this password to log into bandit1 using SSH. Whenever you find a password for a level,**
**use SSH (on port 2220) to log into that level and continue the game.**

<img width="851" alt="Screenshot 2021-07-21 at 6 24 55 PM" src="https://user-images.githubusercontent.com/74819332/126533430-f920ecc5-6134-4aae-b1ce-e637c277520c.png">

go to your terminal and there type :
`ssh bandit0@bandit.labs.overthewire.org -p 2220`

you will get a prompt to enter the password , there type `bandit0` 

<img width="719" alt="Screenshot 2021-07-21 at 6 32 50 PM" src="https://user-images.githubusercontent.com/74819332/126533914-1bd3a9b8-43ae-4217-8530-f5f1ea75e6c9.png">

After that you will enter into the server of Bandit made by overthewire 

<img width="680" alt="Screenshot 2021-07-21 at 6 33 03 PM" src="https://user-images.githubusercontent.com/74819332/126534207-570ab4c9-49b9-487f-873a-78bb769d1c36.png">

now use the command `ls` , which lists all the directories in the current working directory you are in ( Use `pwd` to view the current directory you are in )

<img width="573" alt="Screenshot 2021-07-21 at 6 39 17 PM" src="https://user-images.githubusercontent.com/74819332/126534653-02cba900-2158-4d0c-99e0-2c9d50bedca9.png">

you can see that a file named `Readme` is there as told to us in the problem statement

use the command `cat` which prints out the data of the file 

<img width="570" alt="Screenshot 2021-07-21 at 6 39 35 PM" src="https://user-images.githubusercontent.com/74819332/126535000-bdcee8d2-b188-4b19-9eaa-929dc3762627.png">

Viola , here's the password to level 1 ( I have attached a file which contains password of every problem ) 
