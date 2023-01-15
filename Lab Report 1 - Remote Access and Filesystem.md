# Lab Report 1 - Remote Access and Filesystem

**By Pranav Prabu**

> For this tutorial, every step is done through MacOS.

## Installing Visual Studio Code
![Image](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Visual_Studio_Code_1.35_icon.svg/1920px-Visual_Studio_Code_1.35_icon.svg.png)
The first step necessary for connecting with remote access is installing the Visual Studio Code IDE. This gives you access to an easy-to-use terminal to interface with the remote server.

To install the Visual Studio Code IDE, go to the [VS Code website](https://code.visualstudio.com/) and download the installer that is compatible with your computer's operating system. After downloading the installer, run the installer. After running the installer and opening the application, your screen should look similar to this:

---
<img width="1680" alt="image" src="https://user-images.githubusercontent.com/122483969/211908586-3f6ebffb-5ced-4e51-90cc-d35ec89941e9.png">

---
Then go to the top bar and click on Terminal, and then click on New Terminal.

---
<img width="1679" alt="image" src="https://user-images.githubusercontent.com/122483969/211910039-b42acb5b-2a0a-4adb-acef-eba067771570.png">

---

## Connecting to the Remote Server
After installing VS Code, the next step is to connect to the remote server. First, you need to get your user account name and password from the [Account Lookup website](https://sdacs.ucsd.edu/~icc/index.php). You can get your ID and password by entering in your username from your school email address and your PID (Make sure to use a lowercase a when typing in your PID). After getting your account information go to your terminal in VS Code and enter

`ssh *your CSE 15L account ID goes here*`

The terminal will then ask for your password. Enter your password, and you should be connected to the remote sever. Overall, the process should look something similar to this:

---
<img width="516" alt="image" src="https://user-images.githubusercontent.com/122483969/212523635-5c8fa2a6-869b-4938-ab90-e247b087d098.png">

---

## Running Terminal Commands
After accessing the remote server, you can test out commands through the remote server. Here are some sample commands and what they do:

`cd`
> Allows you to access files in the directory

`ls -a`
> Shows all files within the folder currently accessed by the terminal
<img width="1364" alt="image" src="https://user-images.githubusercontent.com/122483969/212525990-9c6cb7cd-67aa-4dcf-8cbd-4ab82593012e.png">


`ls -lat`
> Shows all files within the folder currently accessed by the terminal along with additional information
<img width="546" alt="image" src="https://user-images.githubusercontent.com/122483969/212526016-50428e2f-e0e9-46b7-be76-f48e94a81806.png">


`ls <directory>`
> Shows files within the directory specified by the user

`exit`
> Exits the remote server terminal
<img width="266" alt="image" src="https://user-images.githubusercontent.com/122483969/212526025-fe6b6b7c-d6c8-4757-ae86-6400a96f00ca.png">

## Conclusion
Congrats! You have accessed your CSE 15L account for the first time, and used commands within the remote server! Good luck with your future work in CSE 15L!
