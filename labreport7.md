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
// These are the commands that were run
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
```

By just pressing `ssh cs15` and then immediately pressing tab, I was able to autocomplete the entire ssh log in statement rather than having to type out the whole thing. 

This allowed me to log back into the ieng6 machine. 



