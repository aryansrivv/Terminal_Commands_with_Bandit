LEVEL 1 ----> LEVEL 2<br/>

logging in to the server by the following command<br/>
`ssh bandit1@bandit.labs.overthewire.org -p 2220`<br/>

<img width="565" alt="Screenshot 2021-07-22 at 1 26 14 PM" src="https://user-images.githubusercontent.com/74819332/126639825-11ca639d-dd90-42e1-b0d6-d6d3a4a395df.png">

here `bandit1` is the username and 2220 is the port number , while `bandit.labs.overthewire.org` is the name of the server\

The problem Statement<br/>

<img width="891" alt="Screenshot 2021-07-22 at 1 30 16 PM" src="https://user-images.githubusercontent.com/74819332/126639406-4b00b6ea-5b61-450d-8223-e1829c8ff200.png">


well , so in the question it says that the password for the next level lies in a file named '-'<br/>
typing the command `ls` we see that there indeed is a file with that name<br/>

<img width="567" alt="Screenshot 2021-07-22 at 1 29 33 PM 2" src="https://user-images.githubusercontent.com/74819332/126639906-c47251e2-e038-452a-88e6-27ead4d1a0ef.png">

you will notice that simply using `cat` command here wont work as the name of the file is not normal<br/>
so what to do : 
There are multiple ways to make the `cat` command read the file <br/>

you can use `cat ./-'` here `./` is used to make the `cat` command understand that the filename might have `-` or even spaces <br/>

<img width="569" alt="Screenshot 2021-07-22 at 1 29 33 PM" src="https://user-images.githubusercontent.com/74819332/126640340-50a48ae3-aedd-4c65-b6f2-4a4a47f56c98.png">


Here you go :) 
you can also use `cat < -` command to read the contents of this file 
