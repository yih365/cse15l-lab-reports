
# Remote Access
## How to log onto a course-specific ieng6 account
  

1. ### Installing VScode
    ![image](Lab1Images\step1img.png)  

    Install VScode (*[here](https://code.visualstudio.com/download)*) in order to use its terminal feature and access the remote server from there. This is my installation of VScode that I downloaded from a browser.

2. ### Remotely Connecting
    ![image](Lab1Images\step2img.png)  

    Use `ssh yourRemoteServer@ieng6.ucsd.edu` to connect to the remote server. Unless the user has an ssh key, the command line will prompt for a password. 

3. ### Trying Some Commands
    ![image](Lab1Images\step3img.png)  

    Here are two unix commands "ls -a" and "pwd". `ls -a` gives a list of all files in the current directory. `pwd` prints the full path of the working directory.

4. ### Moving Files with `scp`
    ![image](Lab1Images\step4img.png)  

    Using `scp [file] [remote server]:[directory]` moves the chosen file into the directory within the remote server. In the above image, I moved my 'index.md' file into the '~/' directory of my remote server.

5. ### Setting an SSH Key
    ![image](Lab1Images\step5img.png)  

    Using `ssh-keygen` within the client and then copying that key to a '.ssh' folder on the server side will allow us to login without typing in a password every time. In the image is an example of a key that is generated through 'ssh-keygen'.

6. ### Optimizing Remote Running
    ![image](Lab1Images\step6img2.png)  

    There are a number of ways we can make remote running easier.  
    In the above image, there are two runs for copying a local edit to "WhereAmI.java" and then running it on the remote server. In the second run, after edting and saving, it took 6 total keystrokes to copy the file to the remote server and run it on the remote server. Using the up arrow key, I accessed the last commands that were run. For copying with the "scp" command, it took 3 keystrokes. And to run the files, it also took 3 keystrokes. Each time, it took 2 keystrokes of the up arrow to get to the appropriate command and 1 keystroke for the 'enter' key.