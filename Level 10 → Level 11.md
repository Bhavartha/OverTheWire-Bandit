# Level 10 → Level 11 #
First of all connect to the shell using

Command: _ssh bandit10@bandit.labs.overthewire.org -p 2220_</br>
Password: _truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk_</br>

### Level Goal ###

The password for the next level is stored in the file data.txt, which contains base64 encoded data

### Commands you may need to solve this level ###

grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd


### Solution ###

We are given a file **data.txt** which contains base64 encoded text

If you aren't familier with base64 encoding then you should search it using your favourite search engine because it's used very often in such type of challenges

To get out password, we **decode** the base64 encoded text

We can use some website like [This really awesome and handy website](https://gchq.github.io/CyberChef) to decode the text or use `base64 -d` to **decode** the text in the terminal
</br></br>
![image](https://user-images.githubusercontent.com/33615252/75613301-0060a100-5b52-11ea-9112-e26e580c6ebf.png)


</br></br>
Password: **IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR**
