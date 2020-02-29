# Level 5 → Level 6 #
First of all connect to the shell using

Command: _ssh bandit5@bandit.labs.overthewire.org -p 2220_</br>
Password: _koReBOKuIDDepwhWk7jZC0RTdopnAYKh_</br>

### Level Goal ###
The password for the next level is stored in a file somewhere under the *inhere* directory and has all of the following properties:

    > human-readable    
    > 1033 bytes in size  
    > not executable
    
    
### Solution ###

As the file we are looking for is human-readable and not-executable, it probably is an ASCII-text file

We know that file is 1033 bytes in size. We can use this information

*Commands you may need to solve this level* says that required commands are: ls, cd, cat, file, du, find

Out of that `du` command is used to view *disk-usage* of files and directories

With appropriate options eg: `du -ba inhere` , we can view size of **all** files inside **inhere** directory in **bytes**</br></br>
![image](https://user-images.githubusercontent.com/33615252/75608393-e80f6880-5af6-11ea-9ed6-468d625f443c.png)

We can then use *|* to give it as an input to `grep` command to filter our results. We can grep for 1033 since we know that the file we are interested in is of 1033 bytes

Now that we know which file contains our key, we can view the contents of the file easily using `cat` command</br></br>

![image](https://user-images.githubusercontent.com/33615252/75608444-5d7b3900-5af7-11ea-8899-c409456eb8f6.png)
