Hello! So today (4/6/23) I took my first lab for CSE 15L. It was quite a nice lab to set things up for this course. I was able to meet my peers, setup my cse15l account, connect to the remote server using that account, running commands in the remote server, and setup my github with my lab report repository. 

# Setting Up Your CSE 15L Account
To log into the remote server for 15l, you first need to reset your password using you account starting with "cs15lsp23" followed by your 2 unique characters. You will need to log in with your UCSD single sign on at [this webpage](https://sdacs.ucsd.edu/~icc/index.php). You should then be able to click on a box with your "cs15lsp23xx" account. After clicking that, you will see a prompt to set your password shown here: ![Image](https://github.com/whatuptj/cse15l-lab-reports/blob/main/Prompt.png)

MAKE SURE TO INPUT YOUR "cs15lsp23xx" ACCOUNT OR ELSE YOU WILL CHANGE YOUR SINGLE SIGN ON PASSWORD LIKE I DID :(. 

# Installing Visual Studio Code
After successfully resetting/creating your password for your CSE 15L account, you will need to install Visual Studio Code, or VSCode for short. VSCode is the program we will be using to access the remote UCSD server. You can find the download and instructions to install VSCode at [this link](https://code.visualstudio.com). After installing VSCode, you may need to install the program [git](https://gitforwindows.org) if you are on a Windows system. Since I am using MacOS, I skipped this step. For a more detailed tutorial you can follow [this link](https://ucsd-cse15l-s23.github.io/week/week1/#due-dates--links) and follow the steps listed under "Part 4 - Remotely Connecting". After installing and opening VSCode you should see something that looks like this: ![Image](https://github.com/whatuptj/cse15l-lab-reports/blob/main/VSCode.png) 

# Accessing the Remote Server
To access UCSD's remote server, you will need to open a terminal in VSCode. To do so, locate the taskbar at the top of VSCode and hover over "terminal". A dropdown should appear along with an option that says "New Terminal". Click that to open a new terminal. It should look something like this: ![Image](https://github.com/whatuptj/cse15l-lab-reports/blob/main/terminal.png)
In this terminal, you can input commands and will use this to navigate the remote server. To login to the remote server, you will input "ssh cs15lsp23xx@ieng6.ucsd.edu" but replace the two xx's with your CSE 15L account letters. Hit enter, then you should be prompted to enter your password that you had set. *Note: you will not be able to see your password or characters being typed in due to privacy concerns.* After entering your password and hitting enter, you should be greeted into the system. ![Image](https://github.com/whatuptj/cse15l-lab-reports/blob/main/server.png)
\
Now in the terminal, you can input some commands. Here are some you can try:
- cd ~
- cd
- ls -lat
- ls -a
- ls <directory> where <directory> is /home/linux/ieng6/cs15lsp23/cs15lsp23abc, where the abc is one of the other group members’ username
- cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/
- cat /home/linux/ieng6/cs15lsp23/public/hello.txt
When you are finished, you can exit the server by using the hotkey Ctrl+D or typing "exit" into the terminal.
  
Congratulations! You have just logged into and used the UCSD remote server!
