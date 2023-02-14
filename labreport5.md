# Lab Report 3

The command that I chose to research was less. The main use for less is to show the file's content. 

## 1. Opening Text Files

The first way we can use the less command is to open up files.

### First Example

In this first example, we use the less command to open up a file called `HandRHawaii.txt`. 

<img width="400" alt="image" src="https://user-images.githubusercontent.com/55414361/218594544-81e19a8f-d8b8-4914-872c-1c941d25dfd1.png">

<img width="485" alt="image" src="https://user-images.githubusercontent.com/55414361/218594609-03ef5475-aa87-4b89-8589-10a30c7ba236.png">

The first picture shows the part where you run the command using less to see the content of the txt file. The second image shows the less command in use. The less command shows us the main content of the file as well as showing the file name and path at the bottom left of the screen. This is useful for us because it allows us to go through all the contents while using less' built in commands to navigate the file. 

Citation: https://phoenixnap.com/kb/less-command-in-linux

### Second Example

<img width="397" alt="image" src="https://user-images.githubusercontent.com/55414361/218594988-d69f7338-26cc-47ba-b64d-3942cd2e5e34.png">

<img width="396" alt="image" src="https://user-images.githubusercontent.com/55414361/218595048-803dc27a-3df8-4c97-a430-468487543103.png">

<img width="1031" alt="image" src="https://user-images.githubusercontent.com/55414361/218595032-d5941a8d-63a6-40f2-8721-449a0177e2e2.png">

In the first picture, I wanted to show what would happen if it we didn't use a proper file while using less. It will tell us that we gave the computer a directory and
will not go inside. The second picture shows me using less in a different file path and opening up a different txt file. The third image shows the content of the 
`ch1.txt` file. The less command is especially beneficial here because this file has so much content, meaning it would take a lot longer to load the whole file. Instead, less will access the file page by page, increasing the loading speed. 

Citation: https://phoenixnap.com/kb/less-command-in-linux

## 2. Searching for a String

Another way we can use the less command is to search for specific strings. 

### First Example
<img width="405" alt="image" src="https://user-images.githubusercontent.com/55414361/218595842-c4923aeb-08da-4184-800e-175154e0c9a8.png">

<img width="441" alt="image" src="https://user-images.githubusercontent.com/55414361/218595696-a06dc56d-fdf2-42ed-bdf0-335b64316440.png">

<img width="436" alt="image" src="https://user-images.githubusercontent.com/55414361/218595775-c3d6bdfd-7671-43bb-b9d8-c9fd31da43c2.png">

<img width="380" alt="image" src="https://user-images.githubusercontent.com/55414361/218595802-1b7b52ec-7628-40c8-bd9a-730efcffe84b.png">

In the first picture, we use the less command to access the file. Then in the second picture we can see the content again. In the third image, I type in a new command 
called `/lagoon`. I use this command in order to look for the word "lagoon". In the fourth picture, we can see the word "lagoon" highlighted in different places. This
command works really well because it allows us to easily access the file and find exactly where the word we are looking for is. 

Citation: https://phoenixnap.com/kb/less-command-in-linux

### Second Example

<img width="395" alt="image" src="https://user-images.githubusercontent.com/55414361/218596198-5537ec9b-c6fc-4780-9c1b-a6970e90a321.png">

<img width="629" alt="image" src="https://user-images.githubusercontent.com/55414361/218596221-8c4739f0-0288-4890-9af7-3788dc3d4770.png">

<img width="414" alt="image" src="https://user-images.githubusercontent.com/55414361/218596248-9abb549c-0a3b-404b-bdaf-524ce3f4d186.png">

<img width="480" alt="image" src="https://user-images.githubusercontent.com/55414361/218596289-354df021-d10f-4672-9cbc-1446203da29c.png">

In the first picture, we use the less command to access the file. Then in the second picture we can see the content again. I typed in a new command 
called `/channel`. I use this command in order to look for the word "channel". This step was just like the previous picture. In the fourth picture we can see the 
word "channel" highlighted in different places. However, I used the command `n` in order to move the page downwards so I could see other content. In the fourth picture, we can see how the word channel is in a different spot. This allows us to see the required word in many different places and allow us to see exactly where the word is. 

Citation: https://phoenixnap.com/kb/less-command-in-linux

## 3. Using Pattern Search

Pattern search works similiarly to find except it follows a specified pattern. 

### First Example

<img width="400" alt="image" src="https://user-images.githubusercontent.com/55414361/218597302-03424c53-7634-4786-8597-7354b4bb2234.png">

<img width="447" alt="image" src="https://user-images.githubusercontent.com/55414361/218597279-12c8b637-acc6-420c-8143-467c72e112aa.png">

In the first picture, we use a new command. The main difference is the `-proom`. What this command does is it highlights the word that comes after `-p`. In this case it is the word "room". In the second picture, we can see where all the "room"s are highlighted since that was the pattern we wanted to find. This works similiarly to the find command except we can immediately declare that we want to want to find a specific word rather than search it in the `less` content. 

Citation: https://phoenixnap.com/kb/less-command-in-linux

### Second Example

<img width="398" alt="image" src="https://user-images.githubusercontent.com/55414361/218611003-71f5eacb-dbf1-4570-b57c-6b480ae1994f.png">

<img width="321" alt="image" src="https://user-images.githubusercontent.com/55414361/218610979-70ab297d-fa1a-4460-a8ba-db7fd1d7a756.png">

<img width="401" alt="image" src="https://user-images.githubusercontent.com/55414361/218611071-51a40232-00f3-4b03-9d79-043aa1a4ef25.png">

<img width="312" alt="image" src="https://user-images.githubusercontent.com/55414361/218611058-8cc76d41-c8fb-4027-85d3-e7ba6062a84e.png">

In the first picture, I do the same thing as the first example except I include a word that doesn't exist in the file. In the second picture we can see that the output tells us that the word doesn't exist in the file. Then I show a proper word in image 3 and show the output in image 4. This is important that the `less` command tells us that it doesn't exist because otherwise we would have to scan the entire document to even see if the file has the word. 

Citation: https://phoenixnap.com/kb/less-command-in-linux

## 4. Opening up Multiple Files

We can also open up multiple files using the `less` command so that we don't have to keep switching files to look for something. 

### First Example  

<img width="584" alt="image" src="https://user-images.githubusercontent.com/55414361/218614556-92af83df-4f55-46f4-90ad-973fe44dda11.png">

<img width="1038" alt="image" src="https://user-images.githubusercontent.com/55414361/218614596-510b65a8-be4f-49d8-ab20-8d46bea6b3d4.png">

<img width="397" alt="image" src="https://user-images.githubusercontent.com/55414361/218614621-24b711ca-6311-442f-9013-c23b5396486d.png">

<img width="434" alt="image" src="https://user-images.githubusercontent.com/55414361/218614691-e9608ab4-2592-4a39-b7bd-3a5612bd9b4c.png">

In the first image, we can see the command which is simply just putting 2 files next to each other. In the second picture we can see there there is File 1 of 2 telling us that we are currently looking at two files. In the third picture, we can see that we reached the end of the first file. After I see this, I use the command `:n` to move to the next page, as we can see in the 4th picture. This is important because we can easily look at the contents of two files and use other commands to decipher each content in the way we want to (find words, etc.). 

Citation: https://phoenixnap.com/kb/less-command-in-linux

### Second Example 

<img width="864" alt="image" src="https://user-images.githubusercontent.com/55414361/218615251-4eccb6a7-8831-4160-bf57-a4bb58bb15fc.png">

<img width="380" alt="image" src="https://user-images.githubusercontent.com/55414361/218615180-0a98a9fb-6fc5-4a0e-93b3-fed42dd9758f.png">

<img width="426" alt="image" src="https://user-images.githubusercontent.com/55414361/218615207-051ac4b5-496c-46b8-8c6c-830fd2296a11.png">

<img width="440" alt="image" src="https://user-images.githubusercontent.com/55414361/218615231-18b2317d-c4d8-4980-9526-71ccbf667624.png">

This process is the same thing as the first example, except I used three files instead of two. In the first picture, I execute the command using three different file paths. In the second picture, we can see that we are in file 1 of 3. In the next picture we can see that we are in file 2 of 3. Finally, in the last picture, we can see that we are in file 3 of 3. This is really important because we can keep as many files as we want and easily cycle through them. This will make the ease of access much better and make it easier for us to traverse through files. 

Citation: https://phoenixnap.com/kb/less-command-in-linux
