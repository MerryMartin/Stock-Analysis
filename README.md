# Stock-Analysis

## Overview of Project

A friend of mine, Steve, has just started his career and asked me for some help with analyzing green stocks so he can diversify funds for his parents.  Although his parents are currently only interested in a small number green stocks, he wanted a tool that would work for the entire stock market and could be executed quickly.  I originally created an analysis script that would analyze twelve different stock tickers.  In order to scale it up to be able to analyze the entire stock market, I needed to reafactor the script to be more efficiant.  

## Results
Using images and examples of code, compare the stock performance between 2018 and 2018 as well as the execution time for the original and refactored script

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
The data outputs for the refactored script matched the outputs for the original script but were executed much faster.  

![VBA_Challenge_2018_dataoutput](https://user-images.githubusercontent.com/115426070/198074389-bb3aba83-3db8-4278-b1db-1bfa18a70e65.png)


## Summary
1 What are the advantages and disadvantages of refactoring code
2 How do these pros and cons apply to refactoring the original VBA script




