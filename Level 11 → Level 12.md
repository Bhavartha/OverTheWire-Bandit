# Level 11 → Level 12 #
First of all connect to the shell using

Command: _ssh bandit11@bandit.labs.overthewire.org -p 2220_</br>
Password: _truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk_</br>

### Level Goal ###

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

### Solution ###

We are given a file **data.txt** where letters have been rotated by 13 positions to form cipher-text

We can again rotate then by 13 positions (13+13=26 - no. of alphabets in english) to get our readable message

Remember the [website](https://gchq.github.io/CyberChef) I mentioned in the previous solution? Lets use that to get work done really fast

In the input section paste the contents of file **data.txt**

In the receipe we choose ROT13 (Rotate 13 cipher)

</br></br>
![image](https://user-images.githubusercontent.com/33615252/75613415-7c0f1d80-5b53-11ea-990d-ff7c111fd484.png)
</br></br>

Password: **5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu**
