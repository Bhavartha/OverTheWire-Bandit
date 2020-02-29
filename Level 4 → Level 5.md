# Level 4 → Level 5 #
First of all connect to the shell using

Command: _ssh bandit4@bandit.labs.overthewire.org -p 2220_</br>
Password: _pIwrPrtPN36QITSp3EQaw936yaFoFgAB_</br>

### Level Goal ###
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

### Solution ###

We can use `file` command to view the types of the files

We can see that only one file contains ASCII text (readable text)

We can now use `cat` command to view contents of that file</br></br>

![image](https://user-images.githubusercontent.com/33615252/75607612-e93d9700-5af0-11ea-8654-d251c03e7b74.png)
