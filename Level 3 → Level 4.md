# Level 3 → Level 4 #
First of all connect to the shell

Command: _ssh bandit3@bandit.labs.overthewire.org -p 2220_</br>
Password: _UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK_<br>

# Level Goal #
The password for the next level is stored in a *hidden file* in the *inhere* directory.

# Solution #
Files that are hidden begin with a *.* before their name eg: `.hidden`

We can still view the contents of the *hidden* file if we have the read permission (which we do have i this case).

We can do someting like:

`cat inhere/.hidden`</br></br>

![image](https://user-images.githubusercontent.com/33615252/75607488-a7f8b780-5aef-11ea-822a-38479bdf3cc7.png)
