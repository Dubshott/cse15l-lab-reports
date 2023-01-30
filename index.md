# Logging into a Course-Specific Account

---
[LabReportWeek3](/labreport3.md)

Logging into the course-specific account is really important because it allows students to log into the school and start running commands within it for their classes. We will be learning how to log into the course-specific account on ieng6. 

## Step 1 - VSCode

We need to first find a place where we can use the terminal and log into both your own computer and the school. To do this, we will be using a software called Visual Studio Code, also known as VSCode. To install this, go to this [website](https://code.visualstudio.com/). 

You should see this: 

![VSCode](vscode download.png)

Select the "Download for Windows" and install the program. Once you finishing installing the program, you should see this pop up:

<img width="767" alt="image" src="https://user-images.githubusercontent.com/55414361/211926600-dd216a6d-176b-4544-8354-64137384772e.png">

## Step 2 - Using Bash

`Git Bash` will be the terminal that we will be we will be scripting with. In order to download gitbash, go this link and download it. [Git Bash](https://gitforwindows.org/)

If you are on Mac, you don't need to do this step because you will already have it preinstalled. However, Windows users need to download this. 

Once you have downloaded `Git Bash`, you need to open the terminal on VSCode. To do this, click "Terminal" at the top of VSCode. Then press "New Terminal"

<img width="436" alt="image" src="https://user-images.githubusercontent.com/55414361/214400229-7a358754-4dfe-47df-9373-642ae4bb3bfa.png">

If you do that, you should see this: 

<img width="770" alt="image" src="https://user-images.githubusercontent.com/55414361/211927352-2badbeca-7ab6-4d63-b60b-fd9897567d01.png">

Once we pulled up the terminal, we need to do the following steps to change the normal VSCode scripting to bash scripting:

1. Use the command Ctrl + Shift + P.  This should create a drop down menu. 

<img width="766" alt="image" src="https://user-images.githubusercontent.com/55414361/211927693-5a0bbcfd-ff3c-4091-8303-95c673a00427.png">

2. In that search bar type in "Select Default Profile" and click it. 

3. Select `Git Bash` 

<img width="448" alt="image" src="https://user-images.githubusercontent.com/55414361/211928089-2d5604d3-84ef-4c6f-bee3-2f9df95df772.png">

4. Now down in the terminal there is a plus button. Press that. 

<img width="733" alt="image" src="https://user-images.githubusercontent.com/55414361/211928246-ad4b3f28-2ce5-4e58-818c-85ba3b4f3606.png">

5. Great! We have our Bash terminal ready. You can also switch between the different terminals and create more terminals if you want. 

## Step 3 - Logging In

Awesome sauce! We have finished the setup process for logging into the account. Now all we need to do is log into the account. 

To find your account, you have to go through a couple steps. 
1. Go to https://sdacs.ucsd.edu/~icc/index.php to look up your CSE15L account
2. You will be able to find your username which should say cs15lwi23***. 
3. Then, look at your results. 
4. At the top there will be a link that states "change your password". Select this link. 
5. Now change put in your current password for your school account and set it to another password. You can even use your same password. 
6. In this step, you can select "NO" for "Change MyTritonLink password?" and set "Change course-specific account passwords?" to "YES". However, you might not even see these options. If that is the case, then you don't have to do anything here. 
7. Press the input that says "Confirm Password" and press the ENTER key. DO NOT press Check Password because it will not work. 
8. Wait a couple minutes for the account to set up and then you should be good to go. 

We are going to first type in this to get logged in: `$ ssh cs15lwi23***@ieng6.ucsd.edu`. Make sure you change the *** to whatever letters are in your username. 

<img width="211" alt="image" src="https://user-images.githubusercontent.com/55414361/211929457-ec26904f-6800-43b3-bdac-c4bd86ee3ef0.png">

If this is your first time, you will recieve an error which is perfectly okay! Just type in "yes" and let it run. 

<img width="447" alt="image" src="https://user-images.githubusercontent.com/55414361/211929640-b7a04d63-972d-4aa7-939a-3367b12463ca.png">

Now go ahead and type in your password. 

Once you properly log in, you should see something like this: 

<img width="397" alt="image" src="https://user-images.githubusercontent.com/55414361/211929749-f50b84ab-57f2-4065-8aa3-83438cde2699.png">

If this is what you see, then congratulations! You successfully logged into your account! Now you can go ahead and run whatever command you want like `cd` or `ls -a` or whatever else you would like to do. 

Hooray!

## Step 4 - Testing

Now we can start using commands. There are way too many commands, so I can't type them all down. However, here are some examples of some commands: 

<img width="576" alt="image" src="https://user-images.githubusercontent.com/55414361/211930178-6af42184-1f5b-4ba7-9553-265c2e975445.png">

<img width="447" alt="image" src="https://user-images.githubusercontent.com/55414361/211930318-8c5a960d-0ba4-41db-978b-1405dd2a6b7a.png">

In addition to these two examples, I also used a couple more such as: 

`cd ~`
`cd`
`cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/`

These commands allow us to go through the directories within the ucsd server. We can create new files for everyone to see and even change other's files. It's basically one huge storage unit for everyone in ucsd to use. 

A couple of the outputs seemed kind of off to me because I didn't have the files associated with the command. For example, the `cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/` didn't properly work for me because I didn't have the right file to open. 

Yay!











