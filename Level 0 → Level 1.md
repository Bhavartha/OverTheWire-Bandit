<h1>Level 0 → Level 1</h1><hr>

First of all connect to the shell<br>
Command: _ssh bandit0@bandit.labs.overthewire.org -p 2220_<br>
Password: _bandit0_<br>

<h3>Level Goal</h3>
The password for the next level is stored in a file called **readme** located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

<h3>Solution</h3>
Since we know that the file __readme__ contains the password,we can use the `cat` command to view the contents of the file
![cat command](https://github.com/Bhavartha/OverTheWire-Bandit/blob/master/images/0-1_1.png?raw=true)

