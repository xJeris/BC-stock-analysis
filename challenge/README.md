# VBA Code Refactoring Analysis

## Overview of Project

The goal of this analysis was to observe the impact refactoring can have on code. This includes any code enhancements, as well as any negative impacts. For this analysis we started with a working VBA script that aggregated data about various stocks by year. We then refactored that code in an attempt to reduce its run time, while still providing the same output.

## Results

The main change made to the code was to reduce the number of times the script needed to access the stock data. In our initial script you can see that we are accessing the year data for each stock separately. Meaning we are gathering data 12 separate times and then aggregating it into the final results grid. This resulted in overall run times of about 1 second for each run.

#### Original Code
<img src="https://raw.githubusercontent.com/xJeris/BC-stock-analysis/main/challenge/resources/VBA_Challenge_OrignalCode.png" width="482">

#### Original Run Times
<img src="https://raw.githubusercontent.com/xJeris/BC-stock-analysis/main/challenge/resources/VBA_Challenge_OrignalTimes.png" width="369">


In the refactored code you can see that we now collect all of the stock data in a single pass of the yearly data. Because of this, the run times were reduced to between 1 and 2 tenths of second. A run time speed improvement of about 84%.

#### Refactored Code
<img src="https://raw.githubusercontent.com/xJeris/BC-stock-analysis/main/challenge/resources/VBA_Challenge_NewCode.png" width="527">

#### Refactored Run Times
<img src="https://raw.githubusercontent.com/xJeris/BC-stock-analysis/main/challenge/resources/VBA_Challenge_2017.png" width="360">
<img src="https://raw.githubusercontent.com/xJeris/BC-stock-analysis/main/challenge/resources/VBA_Challenge_2018.png" width="351">

### Summary

In summary, the refactoring of our code lead to run time improvements. However, it could have included other benefits as well. Examples are:
* Functionality enhancements
* Bug fixes
* Improved code writing and commenting

While this analysis did not see any drawbacks to the refactoring of our code, they do exist. Some examples of these negative impacts are:
* Introduction of new bugs
* Cost prohibitive
* Time consuming

