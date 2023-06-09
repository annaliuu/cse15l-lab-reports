# Lab Report 1

## Step 1 - Installing VScode
To install VScode, you go to the [Visual Studio Code website](https://code.visualstudio.com/) and follow the [download](https://code.visualstudio.com/Download) instructions. There will be different download options for you to choose from depending on your OS (mac, windows, etc). Once it installs, you can open up the program and you'll see something similar to this image below:
![image](sc1.png)

## Step 2 - Remotely Connecting
To begin the remote connection process, go to VScode and open up a terminal through there. You will then type the following command, replacing `zz` with the letters in your specific account:
```
$ ssh cs15lsp23zz@ieng6.ucsd.edu
```

Once you have done so, your screen should look something like this (if there is a message that asks if you would like to continue connecting, say yes):
![image](sc2.png)

Now, you have successfully connected to the remote server and any conmmand that you run will also run on a computer in the CSE basement!

## Step 3 - Trying Some Commands
There are various commands that you can run through the terminal, such as `cd`, `ls`,` ls -lat`, `pwd`, among many others. Here is an example of what running these commands would look like:
![image](sc3.png)

For example, running `cd` stands for "change directory", and changes the directory you are currently in, running `ls` lists all the folders and files in your current directory, and running `pwd` prints the path to the current working directory.
