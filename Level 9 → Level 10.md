# Level 9 → Level 10 #
First of all connect to the shell using

Command: _ssh bandit9@bandit.labs.overthewire.org -p 2220_</br>
Password: _UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR_</br>

### Level Goal ###
The password for the next level is stored in the file data.txt in one of the few human-readable strings, beginning with several ‘=’ characters.

### Commands you may need to solve this level ###

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd


### Solution ###

We are given a file **data.txt**

If we try to use `cat` command to view its contents, we get ����N�� D͜��*'dZ�!!

Not very helpful.

Thankfully `strings` commands helps us to extract readable **strings** from ���G��-0���@��^R�l�"S�

We can now filter this data using `grep`. We know that the data of our interest begins with several **=**

So we grep for **===**</br></br>

![image](https://user-images.githubusercontent.com/33615252/75613176-9f849900-5b50-11ea-97ef-97d674339d83.png)

</br></br>

Password: **truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk**
