## LEVEL 5 ----> LEVEL 6
Welcome to the level 5 of Bandit <br/>

Problem Statement : 

<img width="850" alt="Screenshot 2021-07-27 at 8 58 58 AM" src="https://user-images.githubusercontent.com/74819332/127118372-4d0b7ead-d03e-4237-8062-d68de1dc574d.png">

Now using `cd` and `ls` we find out that there are many directoies here and the file we need can be in any of them <br/>

<img width="1440" alt="Screenshot 2021-07-27 at 9 02 48 AM" src="https://user-images.githubusercontent.com/74819332/127120672-9bece072-b1c2-4a49-a302-97ed21ef2de0.png">

since there are many directories we cannot use file command one by one in each , hence we will use `find` command which is used to find a particular file 



now there are 3 properties given of the file we need , if we use only one of them we will get all the files which follow that trait <br/>

<br/>
luckily here in this level , only one file is there which has the size `1033c` , so using `find ./ -size 1033c` will give the desired result <br/> <br/>
However , if you use `find ./ ! -executable` which lists out all the files which are not executable , we will get a long list in which our file also must be there <br/> 

<img width="571" alt="Screenshot 2021-07-27 at 9 11 55 AM" src="https://user-images.githubusercontent.com/74819332/127121214-800bb97f-3402-4427-add7-dee7940765bc.png">


using all the three properties together we will get our file <br/>
`find ./ -type f -size 1033c ! -executable` 

<img width="562" alt="Screenshot 2021-07-27 at 9 13 04 AM" src="https://user-images.githubusercontent.com/74819332/127121360-1117f763-3160-420d-957e-e289e8821409.png">


We find out that our file is in `maybehere07` directory <br/>
using `cat` and writing out it's location we get our password <br/>
<img width="517" alt="Screenshot 2021-07-27 at 9 14 00 AM" src="https://user-images.githubusercontent.com/74819332/127121494-932600d1-13f4-4db7-947f-432eae447751.png">
