Name               : Vishwa Swami
Date of Submission : 28/09/2026

My Approach

Task-1 : **even_or_odd()** function tests conditional statements (if-else) & modulo operator (%).  
&emsp;&emsp;&emsp;So it returns "even" if number n is divisible by 2 and remainder is zero, unless returns "Odd".  
&emsp;&emsp;&emsp;Edge Case Handling:  
&emsp;&emsp;&emsp;**Negative numbers:** -4 % 2 produces 0 and -5 % 2 produces 1, so modulo arithmetic works for both positive and negative values.  
&emsp;&emsp;&emsp;**Zero:** 0 % 2 = 0, correctly categorizing 0 as "Even".  
&emsp;&emsp;&emsp;**Input validation:** Because Python treats booleans as integers (True == 1, False == 0), because boolean is subclass of integer in python.  
&emsp;&emsp;&emsp;For that we can add -  
&emsp;&emsp;&emsp;if type(n) is not int:  
&emsp;&emsp;&emsp;&emsp;raise TypeError("Input must be a valid integer, not bool or other types."  

Task-2 : **add_all()** function tests for loop and accumulator variable.  
&emsp;&emsp;So, it returns sum of all numbers in a list, provided that collection is a list unless it throws error.
         
