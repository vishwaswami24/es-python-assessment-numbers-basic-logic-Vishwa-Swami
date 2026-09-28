Name               : Vishwa Swami  
Date of Submission : 29/09/2026

**My Approach**

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
Before processing any elements, create an accumulator variable (total = 0) to hold intermediate sums.  
A for loop accesses each element in the input list one by one, from the first index to the last.  
During every iteration, the current item is added to the running total (total += item), updating the stored value in place.
Once the sequence has been completely traversed, the loop terminates, and the function returns the final value stored in total.
So, it returns sum of all numbers in a list.  

**Edge Case Handling:**  
**Empty lists ([]):** The for loop never executes its body because there are no elements to visit. The function returns the initial total of 0.  
**Mixed numeric types:** Adding integers and floats naturally triggers Python's numeric type promotion (e.g., 5 + 2.5 becomes 7.5).  
**Other elements:** If an item inside the list is a string or dictionary, attempting addition would cause an unintended failure,  
making pre-check type validation useful for clean error reporting.  

If the collection is needed to be a list, then we can add in code function -  
if not isinstance(numbers, list): #checks whether an object is an instance of any particular class or not  
&emsp;raise TypeError(f"Expected a list, got {type(numbers).__name__}")
