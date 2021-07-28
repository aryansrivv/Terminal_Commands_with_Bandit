## Level 6 -----> Level 7 

Problem statement : <br/>

<img width="860" alt="Screenshot 2021-07-28 at 8 56 40 AM" src="https://user-images.githubusercontent.com/74819332/127286017-68d845ed-c226-4d21-b244-7a92d3478c78.png">

 
Now in this question we don't have the `inhere` directory , instead the file can be anywhere in the whole root diretory.<br/>

doing `find` command from root directory or heading towards root directory by `cd /` and then doing find command <br/>

`find / -user bandit7 -group bandit6 -size 33c` <br/>


<img width="1440" alt="Screenshot 2021-07-28 at 9 06 40 AM" src="https://user-images.githubusercontent.com/74819332/127288753-e546825b-330c-49e1-ac4b-a2254cb1e1af.png">


You will see that there are many files which show `permissison denied` <br/>

However I have highlighted the file which doesn't show that and has our password <br/>

If you want the permission denied files to dont show use `2>/dev/null` after typing the find command specifics <br/>

<img width="571" alt="Screenshot 2021-07-28 at 9 09 56 AM" src="https://user-images.githubusercontent.com/74819332/127289175-5516a4d6-6944-4a7d-aa37-ae415b634e9e.png">

Use `cat` and then the location of the file to print out the contents of the file. 
