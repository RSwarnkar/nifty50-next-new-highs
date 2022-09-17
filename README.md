# nifty50-new-highs
On an average, How may days and ETF long term investor has to wait to for NIFTY50 to achieve next highs? 

## Waiting period: Statistical Analysis: 

This notebook is statistical analysis for below questions:

## The Questions:
* `Wait Days` : _If I am a Nifty50 ETF investor, how many days on (average, 90%-tile, worst case) I have to wait till nifty50 makes a new high?_ 
* How does the Nifty50 chart looks like if we only plot the next highs and remove all _jaggedness_? 
* How does the distribution of `wait days` look like?

#### Disclaimer: 
Standard Disclaimers apply. Also, this is only statistical anaylsis. **Past performance may not prodict future perfomance.**

## 1.1 Data Collator:

This section collates the individual csv files into a single file in order 
to facilitate the next data processing and analysis.

* Note: We don't have to re-export data from Nifty website. Just fetch it from my [previous github repo](https://github.com/RSwarnkar/nifty50-scrapping) 

## 1.2 Data derivation:

Derive a new column which is date difference. 
This date difference will tell you 
* number of days a long term investor have to wait till the next New High of Nifty50

## 1.3 Data Analysis and Visulization:

## The Answers:
* `Wait Days` : _If I am a Nifty50 ETF investor, how many days on (average, 90%-tile, worst case) I have to wait till nifty50 makes a new high?_ :Do stats.
* How does the Nifty50 chart looks like if we only plot the next highs and remove all _jaggedness_? : Plot using plotly.
* How does the distribution of `wait days` look like? Plot sorted chart. Plot histogram. 

#### Additional exploratory analysis:
* To What distribution given `Days` data confirms to? 
