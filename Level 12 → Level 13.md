# Level 12 → Level 13 #
First of all connect to the shell using

Command: _ssh bandit12@bandit.labs.overthewire.org -p 2220_</br>
Password: _5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu_</br>

### Level Goal ###

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

### Solution ###

We create a tmp directory and convert the given hexdump to file using `xxd`

![image](https://user-images.githubusercontent.com/33615252/83330571-7093d580-a2ad-11ea-9faf-92c11efb2e6c.png)
<br>

Then we check the type of file using `file` command and
- Using `gzip` to extract .gz files
- Using `bzip2` to extract .bz files
- Using `tar` to extract POSIX tar achives

![image](https://user-images.githubusercontent.com/33615252/83330721-c9b03900-a2ae-11ea-8305-408caa2bd54a.png)
<br>
![image](https://user-images.githubusercontent.com/33615252/83330824-7094d500-a2af-11ea-939f-9be5f98be07a.png)
</br></br>

Password: **8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL**
