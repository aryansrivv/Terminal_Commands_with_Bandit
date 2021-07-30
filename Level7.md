# LEVEL 7 ----> LEVEL 8 

<img width="800" alt="Screenshot 2021-07-29 at 7 42 59 PM" src="https://user-images.githubusercontent.com/74819332/127678001-0069a69b-d6d0-4647-a0d8-ac0c437102b4.png">

`ssh bandit7@bandit.labs.overthewire.org -p 2220` <br/> 
Password : `HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs`

if you use `cat data.txt` you will see a almost never ending file printing , so you have to exit the process and start the server again <br/> 

<img width="1440" alt="Screenshot 2021-07-29 at 7 47 18 PM" src="https://user-images.githubusercontent.com/74819332/127679121-e4f5f43a-3a53-44d5-91bb-f6653b1ad239.png">

So you have to find a command that goes in and prints out the required information given the hint that it exists next to the word `millionth`<br/> 

use the `grep` command <br/> 
`grep millionth data.txt` <br/> 


<img width="566" alt="Screenshot 2021-07-30 at 4 51 16 PM" src="https://user-images.githubusercontent.com/74819332/127679287-85485061-f6e3-46ae-9ce8-e10fb63a4734.png">
