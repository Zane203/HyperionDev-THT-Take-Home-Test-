# HyperionDev-THT-Take-Home-Test
## Welcome to my THT Solutions Workspace
This is a repository where you will find my worked solution for the Take-Home-Test from Section A to Section C. Where I have completed a code review for a Java task on Section A. And recently completed a Data Science project for Section B, where I worked on exploring the real-world project repository of Scala that spans data from a version control system (Git) as well as a project hosting site (GitHub). The main aim of this project, for Section B, is to explore The GitHub History of the Scala Language, as I read in, clean up, and visualize different datasets as means to exercise my Data Manupilation skills, as well as Joining Data with Pandas. Moreover, for Section C I have completed a task for Option 4: International Standard Book Numbers, using Python.
## Section A: Code Review - Java Task

***Please take note of the comments next to the algorithms, that are wrapped around by asterisks, as they are pointers to the feedback.***

``` java
public class recursion {
 
	public static void main(String[] args) {
 
		// Saves the string that would be reversed
		String myStr = "emosewA si avaJ";
 
 
		//create Method and pass and input parameter string 
		String reversed = reverse_string(myStr);
		System.out.println("The reversed string is: " + reversed + 
                                   "\nFibonacci Series of 10 numbers:0 1 1 2 3 5 8 13 21 34 "); //1. ***Missing Function Call***
	}
 
 
	//Method take string parameter and check string is empty or not
	public static String reverse_string(String myStr)
	{
		if (myStr.isEmpty()){
		 System.out.println("String in now Empty");
		 return myStr;
		}
		//Calling Function Recursively
		System.out.println("String to be passed in Recursive Function: "+myStr.substring(1));
		return reverseString(myStr.substring(1)) + myStr.charAt(0);}  //2. ***Syntext Error***

	public static <T> void function(T maxNumber) {    //***Invalid name of the function (function keyword)*** 
		// Set it to the number of elements you want in the Fibonacci Series
		int maxNumber = 10; 
		int previousNumber = 0;
		int nextNumber = 1;
		 
	    System.out.print("Fibonacci Series of "+maxNumber+" numbers:");
 
	for (int i = 1; i <= maxNumber; ++i){
	    System.out.print(previousNumber+" ");
	    // On each iteration, we are assigning second number
	    // to the first number and assigning the sum of last two
	    // numbers to the second number
	    int sum = previousNumber + nextNumber;
	    previousNumber = nextNumber;
	    nextNumber = sum;
	    }
 
	}
 
}
```


//Missing Function Call
- This line of code defeats the purpose of the void function that is meant to 
display the Fibonacci sequence, as the function call for displaying the sequence
is missing.

//Syntext Error
- The logic behind the reverse_string() function is correct and accurate, however, 
due to the misspelled function call (reverseString instead of reverse_string), this 
results to a syntex error.

//Invalid name of the function
- The name of a function is usually an action word which describe what the function does, 
not the 'function' keyword itself, and since the purpose of this function is clear, it
should simply be an integer type. Other than that, the logic behind the function looks fine.

## Section B: Personal Project
