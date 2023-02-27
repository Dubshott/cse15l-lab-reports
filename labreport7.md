# Week 7 Lab Report

## Setup (SSH):
Before we start the challenge, we need to set up some things for our SSH so that we won't have to type in the password every single time when logging into our ieng6 account. In addition to this, I also connected the ieng6 account to github so that I don't have to provide authentication when I push or pull. This was all done with steps 1 to 3. 

Here is a picture of me running ssh to log into ieng6 without having to type in a password:

<img width="552" alt="image" src="https://user-images.githubusercontent.com/55414361/221454135-75ca8e2a-cc5c-4ab8-a338-9841b2b4e6b3.png">

## Deleting existing forks

This is similiar to the setup since we are removing any copies that we already cloned.

<img width="503" alt="image" src="https://user-images.githubusercontent.com/55414361/221454258-69f41ea5-aead-44d9-923d-12d8f32f14f9.png">

This is the problem we face when setting this up so we need to fix this. 

<img width="552" alt="image" src="https://user-images.githubusercontent.com/55414361/221454600-22974b7f-2b32-45eb-bac2-c8f983f7a0b4.png">

<img width="231" alt="image" src="https://user-images.githubusercontent.com/55414361/221454795-00f8c300-5439-4475-b0e9-49b7d6837f89.png">

```
rm - r lab 7 <enter>
yes <enter>
ls <enter>
```

In short, we use `rm -r lab7` to remove the file and then used `ls` to check if the file was deleted. 

## Forking Repo

1. Select browser (I used Google Chrome) 
2. Go to lab7 repository (https://github.com/ucsd-cse15l-w23/lab7)
3. Click fork button at top right of screen

<img width="342" alt="image" src="https://user-images.githubusercontent.com/55414361/221455307-bf06bfdd-4065-4f2e-a4c7-17c11a461859.png">

This allows us to create a personal copy of the code and tinker with it all we want without messing up the original branch. We didn't have to use any commands for this. 

## Starting the Timer

We want to see how long it takes for us to finish the challenge, so we go to turn on the timer or stopwatch. 

1. Go to browser (I used google chrome)
2. Type in "stopwatch"
3. Hit the start button to start the timer. 

<img width="513" alt="image" src="https://user-images.githubusercontent.com/55414361/221455484-b586eb16-19b7-426a-959c-84fa0e66a216.png">

No commands were used in this step. 

## Logging back into ieng6

We need to log back into our ieng6 machine so that we can access the files inside it and complete the challenge. Since we already used the ssh option during the set up setup, we shouldn't have to wait for too long since we don't have to type a password anymore. 

<img width="552" alt="image" src="https://user-images.githubusercontent.com/55414361/221455727-3e0f917b-cfaa-4d42-a1f9-372cb110fc8e.png">

```
ssh cs15 <tab> <enter>
// Command that ran: ssh cs15lwi23alp@ieng6.ucsd.edu
```

By just pressing `ssh cs15` and then immediately pressing tab, I was able to autocomplete the entire ssh log in statement rather than having to type out the whole thing. In the comment underneath, we can see the command that was run. 

This allowed me to log back into the ieng6 machine. 

## Clone Github Repository

For this step, we are going to be cloning the repository that we are going to be working with. 

<img width="484" alt="image" src="https://user-images.githubusercontent.com/55414361/221456164-ea6038aa-7de6-465d-a44d-151741a5431c.png">

```
git clone <ctrl+c> <ctrl+v> <enter>
// Command that ran: git clone git@github.com:Dubshott/lab7.git
```

For this command, I wasn't able to use `<tab>` at all, so I had to type out the the first part of the command. Then I copied the ssh from github and pasted it back into the terminal. This allowed me to quickly place in the ssh link, allowing for a fast clone. In the comment underneath, we can see the command that was run. 

In short, this command allowed me to clone the repository, lab7. 

## Running Tests

For this step, I needed to run the program and show that the tests failed. 

<img width="543" alt="image" src="https://user-images.githubusercontent.com/55414361/221456845-2130f009-604f-4f01-8d73-13aff0265d8f.png">
<img width="897" alt="image" src="https://user-images.githubusercontent.com/55414361/221456931-08a904bc-789d-4c92-b833-4ec6220475dd.png">

```
cd lab7 <enter>
<up><up><up><up><up> <enter> 
//Command that was run: javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
<up><up><up><up><up> <enter> 
//Command that was run: java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples
```

I had to first cd into the repository, so I used the cd command to go into the repo. Then I used the up key on my keyboard since I already used that command before. I clicked it a couple times since it was kind of high up but then I pressed enter when I saw the command. In the comment underneath the key strokes, we can see the command that was run. 

In short, these commands allowed me to see that the tests had failed, which is part of the challenge. 

## Fixing the Code

In this, we are going to go inside the file and change edit the code so that the tests will pass. 

The pictures below show all the changes: 

<img width="374" alt="image" src="https://user-images.githubusercontent.com/55414361/221459962-e01ed012-4a4a-4edb-a82a-145806160830.png">

<img width="1112" alt="image" src="https://user-images.githubusercontent.com/55414361/221458312-4dd4b428-32f4-4187-b886-719531214511.png">

<img width="121" alt="image" src="https://user-images.githubusercontent.com/55414361/221458371-98198451-ad93-46b6-b13b-37bd5c3588dc.png">

<img width="158" alt="image" src="https://user-images.githubusercontent.com/55414361/221458393-9042e2ec-b5bd-48b8-9bf5-33717d0f7a47.png">

<img width="391" alt="image" src="https://user-images.githubusercontent.com/55414361/221458430-8892488b-c439-4449-8b1b-463c1fe3e3e3.png">

```
nano Li <tab> <enter>
// Command ran: nano ListExamples.java
<down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down>
// Pressed down key 29 times
<right><right><right><right><right><right><right><right><right><right><right><right><right><right>
// Pressed right key 14 times
<backspace>
2
<Ctrl+O>
<enter>
<Ctrl+X>
```

I first used the nano command and tabbed to get into the right file. Then I had to move my cursor to the right part of the code, so I had to use a lot of `<down>` and `<right>`. Then I used the `<backspace>` and the `2` to change the `index1` to `index2`, which would fix the problem. Then I pressed `<Ctrl+O>` and `<Ctrl+X>` to save the file and exit the nano. 

In short, this whole process allowed me to move through the file and quickly change the problem in the code and fix the main problem. I changed index1 to index2, as shown in the pictures above. 

## Re-run Tests

For this step, I needed to run the program and show that the tests passed.

```
<up><up> <enter>
//Command that was run: javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
<up><up><up> <enter>
//Command that was run: java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples
```

Since I already used this command, I simply pressed `<up>` a couple times until the command came up. Then I used the `<enter>` key to run the command.

In short, these two commands run the jUnit tests and show that they pass this time. 

## Committing and pushing
