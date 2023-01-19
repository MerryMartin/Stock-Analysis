# Stock-Analysis

## Overview of Project

A friend of mine, Steve, has just started his career and asked me for some help with analyzing green stocks so he can diversify funds for his parents.  Although his parents are currently only interested in a small number green stocks, he wanted a tool that would work for the entire stock market and could be executed quickly.  I originally created an analysis code that would analyze twelve different stock tickers.  In order to scale it up to be able to analyze the entire stock market, I needed to reafactor the code to be more efficiant.  

## Results

I created a tickerIndex to match the tickers array to three output arrays - tickerVolumes, tickerStartingPrices, and tickerEndingPrices.  This allowed my for loop to run more effiently since it could run through the tickerIndex values instead of looping through all of the tickers individually.   

---

    'Create a tickerIndex to match tcker array to 3 output arrays
    Dim tickerIndex As Integer
    tickerIndex = 0
    
    'Create three output arrays
    Dim tickerVolumes(12)  As Long
    Dim tickerStartingPrices(12)  As Single
    Dim tickerEndingPrices(12)  As Single
---

The data outputs for the refactored code matched the outputs for the original code but were executed much faster.  

### Data Output (Original and Refactored Scripts)
![VBA_Challenge_2017_dataoutput](https://user-images.githubusercontent.com/115426070/198742322-3fb53b48-2767-4e99-9da9-ad28cc4796ab.png)

![VBA_Challenge_2018_dataoutput](https://user-images.githubusercontent.com/115426070/198074389-bb3aba83-3db8-4278-b1db-1bfa18a70e65.png)

### Original Script Run Times
#### 2017
<img width="252" alt="VBA_Challenge_2017_original" src="https://user-images.githubusercontent.com/115426070/198741700-fb1101d9-eb4f-4d7f-9426-348cb3ccc89a.png">

#### 2018
![VBA_Challenge_2018_original](https://user-images.githubusercontent.com/115426070/198074553-3b2feeb9-5a0d-45ab-baa0-c40ce16f8296.png)

### Refactored Script Run Times
#### 2017
![VBA_Challenge_2017](https://user-images.githubusercontent.com/115426070/198741730-ed1e25f5-1710-439e-b2dc-dab1e010ca75.png)

#### 2018
![VBA_Challenge_2018](https://user-images.githubusercontent.com/115426070/198074876-dd197f00-dcca-4952-a648-128b770d5b2f.png)



## Summary
### Advantages and Disadvantages
There are definitely advantages to refactoring code.  When the refactored code doesn't have to needlessly analyze data points repetitively, it is more efficient and can be used for larger datasets.  It can also be refactored to be more user friendly.  In the project for Steve, I added an input box for him to specify the dates that he wanted to analyze and a couple of macro buttons to make it super easy to execute.  One disadvantage to refactoring code is that once you change one aspect of the code, the developer must carefully examine the rest of the code.  Unexpected errors pop up often and must be debugged in order to get the code to work again.  

---
### Reflections on Refactoring the VBA Script
When I refactored the original VBA code, there were many bugs to work through and it was difficult to isolate the problems.  The process did enable me to become more familar with error messages and how to locate the offending code.  Once the code was working properly again, it was clear that it was now more user friendly and could be executed much faster.  I know Steve will be able to easily use it to analyze the green stocks for his parents and also to analyze the much bigger dataset of the entire stock exchange. 




