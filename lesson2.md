---
layout: default
title: 02-Intermediate
nav_order: 4
---

# Lesson 2: Intermediate Operations

## 1. Functions
A function is similar to a script in that it is a list of commands to be executed.  Where it differs, however, is that functions run with a separate workspace (called a *stack*).  By default, the function does not have access to variables in the main MATLAB Workspace and variables in the function's stack will not be accessible from the command line.  
Instead, you pass data into and out of functions when you call them. The function declaration statement (at the top of the function) defines which variables will be passed into and out of it. 
- For example, a function declaration looks something like: 
```
function [output1,output2] = name_of_function(input1,input2,input3)
```

Functions can have any number of input and output variables, and can be named mostly anything (as long as they don't have a special character or a space in them).

Functions are useful when you are interested in only some output variables in a set of commands.  You can also run a function inside of a script (or another function), which makes it a very space and time-saving way to run many commands.  

Functions are called by using their name and the output/input format specified above (see below example). For example, the operation 'mean' is a function.  
- It is called by, e.g. ```[avg] = mean(input);``` where 'avg' is the output variable, 'mean' is the function name, and 'input' is the input variable or value. 

1. Open \Scripts\isleapyear.m. 
- What does it do? How can we use it? 
2. Figure out how to use isleapyear from the command line. 

### B7. Control structures and indexing 
- Create a new blank script

#### For loops
- Loops are handy when you need to repeat a process many times, such as when reading through many rows or columns of data, or running a process iteratively. 
- The **for** function allows you to do this. Learn more by typing into the command window: ```doc for;```
1. In your new script, create a for loop that increments an index **yr** from 1000 to 2020 by 1. 
- within the loop, call the isleapyear function, using the value of yr. Set the function to be verbose. 

#### If statements
- An 'if' statement evaluates if a condition is met (true) or not met (false), and allows the user to perform different functions based on the outcome.  
  - If the statement is true (condition is met) Matlab will execute whatever commands are below it.  
  - If it is untrue, it will
 execute any commands that are below the 'else' statement.
  - Just like 'for' loops, 'if' statements have to be closed with an 'end'
1. Within the existing for loop, add an if statement that checks if two conditions: 
- That the value of **yr** is a leap year (***hint*** you'll use the output from isleapyear)
- That the value of **yr** is a prime number (***hint*** you'll use the function **isprime**)
2. If both conditions are met, use the **disp** function to send a message to the command window.

#### Indexing and the 'find' function
1. Use the **randi** function to create a variable **rand_nums** that is a *10000 x 1* list of random numbers between 1 and 1000
2. Use the **find** function to create a list of: 
- All rows where rand_nums are greater than (>) 500
- All rows where rand_nums is less than or equal to (<=) 100 
- All rows where rand_nums is between 100 and 700
- All rows where rand_nums is exactly 999

#### Creating your own function
3. Finally, make your own function (call it **leap_and_prime**). This function should:
- take an integer year as input 
- check if it is a leap year *and* a prime number
- display a message if both are true.
