# Week 1 Lab Report
In this lab report, I will be walking through the steps to set up the CSE 15L lab environment.

&nbsp;

## **Step 1: Installing VS Code**
___
To install VS Code, first go on their website [https://code.visualstudio.com/](https://code.visualstudio.com/). Then, follow the instructions needed to download on your computer. Make sure to pick the correct operating system for your installment.

![Image](imgs/vscode.png)
*(VS Code home page)*


## **Step 2: Remotely Connecting**
___
To remotely connect, first open the terminal. Then, copy this command "ssh cs15lwi23avu@ieng6.ucsd.edu" to ssh into the CSE Basement server. Lastly, the terminal will prompt you for your password. Enter your password and you will have access to the server.

![Image](imgs/login.png)

*(remotely connecting to server)*

## **Step 3: Trying Some Commands**
___
Lastly, to test that your connection is working, you can try some commands. Some commands include:

* **cd ~:** takes you to the home directory
* **cd:** takes you into a directory
* **ls -lat:** lists all of the files in a directory and the information of each file
* **ls -a:** lists all of the files in a directory, including hidden files
* **ls [directory]:** lists all of the files in a specified directory
* **cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/:** copies the hello.txt file to the home directory
* **cat /home/linux/ieng6/cs15lwi23/public/hello.txt:** prints the contents of the hello.txt file

... and more!

![Image](imgs/lsexample.png)

*(example using ls -a)*

&nbsp;
> (TIP!) Make sure to log out of the remote server using Ctrl-D or by running the command "exit".

![Image](imgs/exit.png)	

*(exiting server)*

&nbsp;

And you're done! Thanks for reading. :)
