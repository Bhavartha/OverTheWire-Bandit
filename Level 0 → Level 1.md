<h1>Level 0 → Level 1</h1><hr>

First of all connect to the shell<br>
Command: _ssh bandit0@bandit.labs.overthewire.org -p 2220_<br>
Password: _bandit0_<br>

<h3>Level Goal</h3>
The password for the next level is stored in a file called **readme** located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

<h3>Solution</h3><br>
Since we know that the file **readme** contains the password,we can use the `cat` command to view the contents of the file<br><br>

![cat command](https://user-images.githubusercontent.com/33615252/75606858-ee96e380-5ae8-11ea-8048-095a08d73feb.png)


