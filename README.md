Check whether a String is Palidrome
In this article  we will see if the string is palindrome or not in java programming language.

A string is palindrome if the reverse and the original string is same

Lets understand this with the help of an example:- 

Input sting:- AMA
Reverse sting:- AMA
Here AMA = AMA so this is a palindrome 

Check whether a String is Palidrome in java
Algorithm
Take a String input from user and store it in a variable called “s”
Take a variable called as “rev” to store reverse value 
Take a i loop and start it from i=s.length()-1 to i>=0
Then get each character one by one using charAt() and store it in “rev” variable
If rev variable is equals to s variable then print String is palindrome else print String is not palindrome
Program to Check given String is Palindrome or Not in java
Code in Java
Run
import java.util.Scanner;

public class StringIsAPalindromeOrNot {

	public static void main(String[] args) {
		
		String s = "arora";
		String rev = "";
		for (int i = s.length()-1; i >=0 ; i--) 
			rev=rev+s.charAt(i);
		if(s.equals(rev))
			System.out.println("String is palindrome");
		else 
			System.out.println("String is not palindrome");

	}

}
Output
String is palindrome
Note
In this java program, we’re going to check string input by the user will be palindrome or not. Take a String input from the user and store it in a variable called “s”. A palindrome string is one that will be the same if we read from forward and from backward also. Strings like ‘madam’, ‘lol’, ‘pop’, ‘arora’ are examples of palindrome string . We’re storing a reversed string in ‘rev’ variable after that we will compare that original string and the reversed string are same or not using equals() method.
Method 2 (Check whether a String is Palidrome)
Here the reverse of the string will be stored and then will be checking if the original and the reverse is same or not.

Run
import java.util.*;

public class Main {
    public static void main(String args[]) {
        String original = "Prepinsta", reverse = "";  // Objects of String class
        
        int length = original.length();
        for (int i = length - 1; i >= 0; i--) 
        reverse = reverse + original.charAt(i);

        if (original.equals(reverse))
            System.out.println("Entered string is a palindrome.");
        else
            System.out.println("Entered string isn't a palindrome.");
    }
}
Output
Entered string isn't a palindrome.
