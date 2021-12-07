# VBA Code Refactoring Analysis

## Overview of Project

The goal of this analysis was to observe the impact refactoring can have on code. This includes any code enhancements, as well as any negative impacts. For this analysis we started with a working VBA script that aggregated data about various stocks by year. We then refactored that code in an attempt to reduce its run time, while still providing the same output.

## Results

The main change made to the code was to reduce the number of times the script needed to access the stock data. In our initial script you can see that we are accessing the year data for each stock separately. Meaning we are gathering data 12 separate times and then aggregating it into the final results grid.

<img src="https://raw.githubusercontent.com/xJeris/BC-stock-analysis/main/challenge/resources/VBA_Challenge_OrignalCode.png" width="482">

<img src="https://raw.githubusercontent.com/xJeris/BC-stock-analysis/main/challenge/resources/VBA_Challenge_OrignalTimes.png" width="369">

### Refactored Time

<img src="https://raw.githubusercontent.com/xJeris/BC-stock-analysis/main/challenge/resources/VBA_Challenge_2017.png" width="480">
<img src="https://raw.githubusercontent.com/xJeris/BC-stock-analysis/main/challenge/resources/VBA_Challenge_2018.png" width="467">

### Summary



