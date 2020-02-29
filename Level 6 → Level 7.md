# Level 6 → Level 7 #
First of all connect to the shell using

Command: _ssh bandit6@bandit.labs.overthewire.org -p 2220_</br>
Password: _DXjZPULLxYr17uwoI01bNLQbtFemEgo7_</br>

### Level Goal ###
The password for the next level is stored somewhere on the server and has all of the following properties:

> owned by user bandit7

> owned by group bandit6

> 33 bytes in size


### Commands you may need to solve this level ###
ls, cd, cat, file, du, find, grep
    
### Solution ###

The file is stored somewhere on the server :worried: and we need to find it :sob: . Doing it manually is almost impossible.

We can use `find` command to find the file on the system. Since it can be anywhere we will search every file :wink:.

We can try doing something like `find /' but that produces insane amount of information :dizzy_face:

We must find a way to filter our results. Using `grep` now would be a little difficult since we dont know the file name. Also using `du` command and then piping it to `grep` might not be as helpful as it was previously because there might be many files in the entire system that are of the specified size.

Lets explore more.... (Remember we know the owners of file and its size)

Searching on the internet and reading man page of find command ( `man find` ) gave us something we can try</br></br>

![image](https://user-images.githubusercontent.com/33615252/75609622-18a8cf80-5b02-11ea-8809-fec5479b1d05.png)
</br></br>

![image](https://user-images.githubusercontent.com/33615252/75609635-455ce700-5b02-11ea-8eec-ac68c1a87f4f.png)

Now we can combine these to get our file</br></br>

![image](https://user-images.githubusercontent.com/33615252/75609667-835a0b00-5b02-11ea-8dc4-9db9dfbf4048.png)


Hmmmm.... Only if we could remove those annoying Permission denied messages.

How?  

Well we can redirect STDERR (standard error) message to /dev/null (Magical device that can vanish everything???)</br></br>

![image](https://user-images.githubusercontent.com/33615252/75609836-b6e96500-5b03-11ea-9d62-7c6f937572cd.png)


Finally we got our password: **HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs**

