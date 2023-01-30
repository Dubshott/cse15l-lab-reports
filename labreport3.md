# Week 3 Lab Report

## Part 1

The first thing we needed to do was create code that would allow us to add new strings and display those strings on the webpage. Here is what that code looks like: 

![image](https://user-images.githubusercontent.com/55414361/215362279-a9ab826a-ee50-4afb-862e-5f099b49ec56.png)

The method that includes all the adding is in `public String HandleRequest (URI url) {`.

Here are the screenshots for using the methods: 

Adding 2 Strings: 

<img width="440" alt="image" src="https://user-images.githubusercontent.com/55414361/215362344-d3e016cd-8d5e-44db-a1bd-3e29fead9fc9.png">

<img width="375" alt="image" src="https://user-images.githubusercontent.com/55414361/215362357-5cc1ea35-03ae-49e4-8781-a9959f43bc9c.png">

Here is the result: 

<img width="214" alt="image" src="https://user-images.githubusercontent.com/55414361/215362378-77ae29f3-eba0-49a5-926f-d03707d2aa3f.png">

The only method that is being called through these examples is in `public String HandleRequest (URI url) {`. All the code to add the Strings is within this method.

The first thing the code will go through is if the webpage is in the default `localhost:4000`. If it is, then it will show the final output of all the strings. If it isn't, 
then it will check the URL path that is inputted. If it follows exactly as `localhost:4000/add-message?s=<input>`, then it will add the input into the `String input`, 
and say, "'input' has been added!". Once we go back to `localhost:4000/`, then we will be able to see the inputted String. 

Therefore, the most relevant arugments are the `String input` and `String[] parameters` since it takes in the in the user's input and displays it on the screen. 

The value that gets changed after the specific request would be String input because it adds on an additional String to display. That is how we are able to see each string
that is inputted. The way we do this is by adding the parameter (the input) and adding a `\n` to the main `String input`.

## Part 2

here is the buggy code: 

``` Java
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```

This first test induces a failure:  

``` Java
  @Test
  public void testReverseInPlaceMultipleNums() {
    int[] input1 = { 2, 3, 4 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{4,3,2}, input1);
  }
```

This second test doesn't induce a failure. 

``` Java
@Test 
	public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}
```

Here are the tests running: 

<img width="602" alt="image" src="https://user-images.githubusercontent.com/55414361/215364373-b88b89f0-8d1f-450b-9e97-70a370a14c06.png">

And now to fix the code: 

Old Version:
``` Java
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```
New Version:
``` Java
  static void reverseInPlace(int[] arr) {

    int temp;
    
    for(int i = 0; i < arr.length/2; i += 1) {
      temp = arr[i];
      arr[i] = arr[arr.length - i-1];
      arr[arr.length-i-1] = temp;
    }
  }
```

The main thing we added was a temporary array that would store each value from the real array. The reason why we did this was because the old code basically started clashing since all the values were constantly being replaced. When we add a temporary array, the variables won't be constantly replaced and will allow for a smooth transition. 

## Part 3

In week 2 and 3 I learned a lot about JUnit tests. Before these weeks, I had no idea what JUnit even was so it was nice to see that there was a way to check your code. The only way I was able to check before was through gradescope when the teacher used an AI grader. Now through JUnit, I can check how my code does and properly debug if there is an error. 


