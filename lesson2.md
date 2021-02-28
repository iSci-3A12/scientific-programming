---
layout: default
title: 02-Intermediate
nav_order: 4
---

# Lesson 2: Intermediate Operations
In this lesson, you will build upon the [basics](lesson1) to create working scripts and functions and perform some analyses. 

## 1. Preparation
1. Make sure your **Working Directory** is set to ```/ > MATLAB Drive > iSci3A12-SciProgramming```. This is where we will run our scripts and analyses. 
1. In MATLAB, open the following files in the **Editor** window: 
  - The script ```iSci_Intermediate.m```, and 
  - The function ```iSci_lucky_numbers.m```
1. Save a copy of ```iSci_lucky_numbers.m``` in the same direcotory and name it ```my_lucky_numbers.m```:
  - With ```iSci_lucky_numbers``` open, click ```Save > Save As...```
  ![Save As Dialog Box](assets/img/saveas.png)
  - Name the new file ```my_lucky_numbers.m```
1. Open ```iSci_Intermediate``` in the Editor window, and follow along with the directions within. 

<table style="background-color: #ffff99;">
<tbody>
<tr>
<td>
<p><b>IMPORTANT NOTE:</b> For this lesson, you will work through the script <b>iSci_Intermediate.m</b>. Most instructions are embedded as comments in the script, and you can run through the steps by highlighting line(s) and executing them in the Command Window with F9.</p>
<p>Additional information on concepts is provided below.</p>
</td>
</tr>
</tbody>
</table>


### B7. Control structures and indexing 
- Create a new blank script

#### For loops
- Loops are handy when you need to repeat a process many times, such as when reading through many rows or columns of data, or running a process iteratively. 
- The **for** function allows you to do this. Learn more by typing into the command window: ```doc for;```
1. In your new script, create a for loop that increments an index **yr** from 1000 to 2020 by 1. 
- within the loop, call the isleapyear function, using the value of yr. Set the function to be verbose. 

#### If statements
- An ```if``` statement evaluates if a condition is met (true) or not met (false), and allows the user to perform different functions based on the outcome.  
  - If the statement is true (condition is met) Matlab will execute whatever commands are below it.  
  - If it is untrue, it will
 execute any commands that are below the ```else``` statement.
  - Just like ```for``` loops, ```if``` statements have to be closed with an ```end```
1. Within the existing for loop, add an if statement that checks if two conditions: 
- That the value of **yr** is a leap year (***hint*** you'll use the output from isleapyear)
- That the value of **yr** is a prime number (***hint*** you'll use the function **isprime**)
2. If both conditions are met, use the **disp** function to send a message to the command window.

#### Indexing and the ```find``` function
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
