---
layout: default
title: 04-Analyze a Station
nav_order: 6
---

# Lesson 4: Analyzing one Station's Data

**Estimated time to complete: 30-90 minutes**  
In this exercise, you will complete the code and comments for the script ```process_adelaide.m``` (which is found in your MATLAB Drive). When completed, this script will load data for the climate station ```Adelaide Airport```, and carry out the same analysis as you completed in a spreadsheet for the first part of your Climate Data Assignment. This should give you a good understanding of the power of scripted approaches, and you'll build on this script to create a final deliverable that can complete analysis for all sites at once. 
  
By the end of this lesson, you will have created the following required deliverable: 
- A script called ```process_adelaide.m```. 

### Video
<iframe width="853" height="480" src="https://web.microsoftstream.com/embed/video/a349dc07-486a-4869-8e6b-ea7ac8d376e3?autoplay=false&amp;showinfo=true" allowfullscreen style="border:none;"></iframe>

## 1. Setup
1. Make sure your **Working Directory** is set to ```/ > MATLAB Drive > iSci3A12-SciProgramming```. This is where we will run our scripts and analyses. 
1. In MATLAB, open the file ```process_adelaide.m```. This script has been mostly completed for you. Your tasks are described below: 

## 2. Your tasks
1. Execute the script line-by-line (hint: use the ```F9``` key, read comments, and view the resulting variables to understand what each line of code is doing.
1. Look for comments that contain ```<**TO DO**>``` and instructions. Complete the code on these lines. 
1. Ensure that the script runs without issues (i.e. by clicking the ```Run``` button) and produces the figures in the \Figs directory.
1. Add comments to the top comment section and on other lines where you've added code. 

## 3. Hints
1. Already included in the function is some code that will remove -9999s from your data. If your timeseries graph shows a steep drop in values (e.g. equal to -9999), you've likely used the wrong variable to calculate anomalies. 

## 4. Deliverables
- Ensure that all changes to your script ```process_adelaide``` is saved.
- **NOTE** that you are submitting the script and not the output (Jay is going to run the script on his computer to evaluate that it creates the proper outputs).

## 5. Head to the next exercise
Now that you've processed one site, the challenge is to generalize this code into a function that can analyze all sites in your data folder at once! Head to the [final lesson](lesson5). One more to go! 
