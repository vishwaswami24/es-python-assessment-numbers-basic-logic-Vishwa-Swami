Name               : Vishwa Swami
Date of Submission : 29/09/2026

My Approach

**Task-1 :**  
**even_or_odd()** function tests conditional statements (if-else) & modulo operator (%).  
So it returns "even" if number n is divisible by 2 and remainder is zero, unless returns "Odd".  
**Edge Case Handling:**  
**Negative numbers:** -4 % 2 produces 0 and -5 % 2 produces 1, so modulo arithmetic works for both positive and negative values.  
**Zero:** 0 % 2 = 0, correctly categorizing 0 as "Even".  
**Input validation:** Because Python treats booleans as integers (True == 1, False == 0), because boolean is subclass of integer in python.  
For that we can add -  
if type(n) is not int:  
&emsp;raise TypeError("Input must be a valid integer, not bool or other types."  

**Task-2 :**  
**add_all()** function tests for loop and accumulator variable.  
So, it returns sum of all numbers in a list.  
If the collection is needed to be a list, then we can add in function -  
if not isinstance(numbers, list): #checks whether an object is an instance of any particular class or not
    raise TypeError(f"Expected a list, got {type(numbers).__name__}")
