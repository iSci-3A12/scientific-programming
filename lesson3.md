---
layout: default
title: 03-Create a Function
nav_order: 5
---

# Lesson 3: Create a Function
**Estimated time to complete: 30 minutes**  
In this mini-lesson, you're tasked with applying the skills you learned in the [previous lesson](lesson2) to create your very own function. By the end of this lesson, you will have created the following required deliverable: 
- A function called ```simple_stats.m```. 

## 1. Setup
1. Make sure your **Working Directory** is set to ```/ > MATLAB Drive > iSci3A12-SciProgramming```. This is where we will run our scripts and analyses. 
1. In MATLAB, open the file ```simple_stats.m```. This function has been started for you to complete the tasks described below: 

## 2. Your task
Full directions are already provided in the top comments of ```simple_stats```. You must add code and comments to ```simple_stats``` so that it: 
1. Takes a column vector of any length as input (n rows x 1 column), which may or may not contain NaNs.
1. Using the inputted column vector, creates a 5x1 column vector as output, which contains the following values: 
  - row 1: minimum value of the inputted column vector (excluding NaNs)
  - row 2: maximum value of the inputted column vector (excluding NaNs)
  - row 3: mean value of the inputted column vector (excluding NaNs)
  - row 4: median value of the inputted column vector (excluding NaNs)
  - row 5: highest prime number (if exists) or NaN if there are no prime numbers in the inputted column vector
1. Has completed comments for the 'usage' and 'created by' information in the top comment section
1. Has comments with each section of code that explains what it does.

### 2.1. Hints
- The function ```nanmean``` (and other similar functions like ```nanmin```) are very handy for filtering out NaNs. Learn more by entering ```doc nanmean``` in the command window. 
- Remember that your *function declaration* will assign the inputted column vector with the internal variable name ```numbers_in```; you will want to perform your calculations on this variable. Similarly, your final (ready to output) variable should be named ```stats``` so that it is passed back to the Command Window.
- Jay will evaluate this function by calling it from the command window with a couple of different vectors as input. 
- If you want to test the output, try running the following in the command window and inspecting the output: 
```
[stats_out] = simple_stats([-9; 234.32; 1; NaN; 203.34; NaN; 87; 63])
```

## 3. Deliverables
- Ensure that all changes to your function ```simple_stats.m``` is saved. **NOTE** that you are submitting the function and not the output (Jay is going to run the function on his computer to evaluate it).

## 4. Head to the next exercise
Once you're done here, head to the [next lesson](lesson4) to start building a script that analyzes weather station data. 
