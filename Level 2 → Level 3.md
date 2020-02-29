# Level 2 → Level 3 #
First of all connect to the shell

Command: _ssh bandit2@bandit.labs.overthewire.org -p 2220_</br>
Password: _CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9_<br>

### Level Goal ###
The password for the next level is stored in a file called `spaces in this filename` located in the home directory

### Solution ###
We can use `cat` command with auto-completions using tabs or escape spaces using backslash 

_cat spaces\ in\ this\ filename_</br></br>


![image](https://user-images.githubusercontent.com/33615252/75607418-d1651380-5aee-11ea-9a0b-daf507c71ed7.png)
