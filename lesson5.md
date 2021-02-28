---
layout: default
title: 05-Analyze all Stations
nav_order: 7
---

# Lesson 5: Analyzing Any or All Stations

**Estimated time to complete: 1.5 hours **  
In this final exercise, you'll take what you learned in the [previous lesson](lesson4) to build a function (```plot_station_data.m```, which has been started for you) that can process any or all station data in your ```/Data``` folder. In completing this function, you will demonstrate the true value of using a scripted approach to create automated, repeatable, and extensible analyses.

By the end of this lesson, you will have created the following required deliverable: 
- A function called ```plot_station_data.m```. 

## 1. Setup
1. Make sure your **Working Directory** is set to ```/ > MATLAB Drive > iSci3A12-SciProgramming```. This is where we will run our scripts and analyses. 
1. In MATLAB, open the file ```plot_station_data.m```. This function has been partly completed for you. Your tasks are described below: 

## 2. Your tasks
In the last lesson, you created a script that processes and plots station data for a single station using a set reference period to calculate anomalies (i.e. 1951-1980). ***But what if you wanted to do the same analysis for other sites? For all sites? What if you wanted to change the reference period and run it again?*** This is where creating a function (where those preferences can be entered as inputs) becomes valuable. 
  
In this task, you need to complete the code in ```plot_station_data``` so that the function: 
- Allows a user to select one site to analyze by entering the name of a station's data file as it appears in ```/Data``` (e.g. ```Arhangelsk```, ```Base Orcadas```, etc.). Internally, this is assigned to the ```station_name``` variable.
- Allows a user to process all site data in ```/Data``` at once (in a loop) if they enter ```all``` in the place of a station file name.  
- Allows a user to specify the start (```ref_start```) and end (```end_year```) years for the *reference period* for calculating anomalies.
- Similar to the previous lesson, creates two png figures for each site: 
  - A *timeseries* figure named ```<stationName>_timeseries.png```, where ```<stationName>``` is the file name of the station data file, and 
  - A *barcode* figure named ```<stationName>_barcode.png```, where ```<stationName>``` is the file name of the station data file.
  
The *function declaration* for ```plot_station_data``` has already been created to accommodate the inputs defined above: 
```
function [] = plot_station_data_soln(station_name, ref_start, ref_end)
```

### 2.1 Hints
- When you are ready to test your function, run each of the following lines in the Command Window separately to see if they create the desired outputs: 
  - ```plot_station_data('Arhangelsk', 1961, 1990)```
  - ```plot_station_data('Kanazawa', 1971, 2000)```
  - ```plot_station_data('all', 1971, 2000)```
  

## 3. Deliverables
- Ensure that all changes to your function ```plot_station_data``` is saved.
- **NOTE** that you are submitting the function and not the outputs (Jay is going to run the script on his computer to evaluate that it creates the proper outputs).

## 4. Reflection time! 

