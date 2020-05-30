# Level 13 → Level 14 #
First of all connect to the shell using

Command: _ssh bandit13@bandit.labs.overthewire.org -p 2220_</br>
Password: _8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL_</br>

### Level Goal ###
The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

### Solution ###

We can simply login as bandit14 using the ssh-key we have

`man ssh` helps us to know how to use the ssh command 

![image](https://user-images.githubusercontent.com/33615252/83331352-6248b800-a2b3-11ea-9dd6-21589ade04da.png)

![image](https://user-images.githubusercontent.com/33615252/83331381-9b812800-a2b3-11ea-8fc4-f4acd72690df.png)

`cat /etc/bandit_pass/bandit14` command after logging in as bandit14 gives us the password


Password: **4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e**
