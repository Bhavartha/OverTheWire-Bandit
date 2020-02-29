# Level 7 → Level 8 #
First of all connect to the shell using

Command: _ssh bandit8@bandit.labs.overthewire.org -p 2220_</br>
Password: _cvX2JJa4CFALtqS87jk27qwqGhBM9plV_</br>

### Level Goal ###

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once


### Solution ###

`uniq` command allows us to find unique lines.

But there is a catch. It filters out the adjacent matching lines. What if there are repeated lines but they arent adjacent?

We wont be able to get the result we desire

Thus we first sort the file using `sort` command. After sorting same lines will be adjacent and thus `uniq` will get it done.

>-u : It allows you to print only unique lines.</br></br>
![image](https://user-images.githubusercontent.com/33615252/75612968-8975d900-5b4e-11ea-8204-791a4f9e8f11.png)
</br></br>

Password: **UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR**
