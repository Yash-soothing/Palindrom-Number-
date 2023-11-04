# Palindrome Number
A palindrome number is a number that reads the same backward as forward. It is a type of magic number in which the digits and/or signs are rearranged to form an identical number.

Examples of palindrome numbers include 121, 333, 444, 555, and 666. 

This is a basic level program in java, where we need to give the input value in the code itself, so that it takes the input and executes the code and identifies whether the number is palindrome or not.

The provided Java code is a simple program designed to determine whether a given integer is a palindrome. A palindrome number is one that remains the same when its digits are reversed. The code uses the number 454 as an example and checks if it qualifies as a palindrome.

In this program, there are several integer variables in use: 'n,' which is initialized to 454, representing the number to be assessed for palindromic properties; 'temp,' which holds a copy of the original number 'n'; 'r,' responsible for storing the remainder when 'n' is divided by 10 during the digit-reversal process; and 'sum,' which accumulates the reversed digits of 'n.'

The code employs a 'while' loop to execute a sequence of operations as long as 'n' remains greater than 0. Within this loop, 'r' captures the last digit of 'n' through the remainder of 'n' divided by 10. 'Sum' is updated by multiplying its current value by 10 and adding the value of 'r,' effectively reversing the digits of 'n.' The loop continues to remove the last digit from 'n' by dividing it by 10.

Following the 'while' loop, the code performs a comparison, checking whether the original number 'temp' is identical to the reversed number 'sum.' If they are equal, this indicates that the original number is a palindrome. Consequently, if 'temp' and 'sum' are found to be equal, the program will output "palindrome number"; otherwise, it will print "not palindrome."

In the case of the code provided, as the original number 'n' is set to 454, and the reversed number 'sum' is also 454, the program will output "palindrome number" to confirm that 454 is indeed a palindrome. You can substitute the value of 'n' with any other integer to test whether it exhibits palindromic characteristics.

class Main{  
 public static void main(String args[]){  
  int r,sum=0,temp;    
  int n=454;//It is the number variable to be checked for palindrome  
  
  temp=n;    
  while(n>0){    
   r=n%10;  //getting remainder  
   sum=(sum*10)+r;    
   n=n/10;    
  }    
  if(temp==sum)    
   System.out.println("palindrome number ");    
  else    
   System.out.println("not palindrome");    
}  
}
