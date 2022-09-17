# Nifty50 next new highs : Statistical Analysis: 
On an average, How may days and ETF long term investor has to wait to for NIFTY50 to achieve next highs? 

This notebook is statistical analysis for below questions:

## The Questions:
* `Wait Days` : _If I am a Nifty50 ETF investor, how many days on (average, 90%-tile, worst case) I have to wait till nifty50 makes a new high?_ 
* How does the Nifty50 chart looks like if we only plot the next highs and remove all _jaggedness_? 
* How does the distribution of `wait days` look like?
* Additional exploratory analysis 1: Possible to check to what kind of distribution given `Days` data confirms to? 
* Additional exploratory analysis 2: Can you generate and artificial distribution for such data? 

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

## 1.3 Algorithm:

* `Wait Days` : _If I am a Nifty50 ETF investor, how many days on (average, 90%-tile, worst case) I have to wait till nifty50 makes a new high?_ 


* How does the Nifty50 chart looks like if we only plot the next highs and remove all _jaggedness_? : Plot using plotly.
* How does the distribution of `wait days` look like? Plot sorted chart. Plot histogram. 

## 1.4 Data Visulization: 

![image](https://user-images.githubusercontent.com/24961188/190855600-137683aa-e510-448d-90d5-bdd61d1bedf7.png)
![image](https://user-images.githubusercontent.com/24961188/190855608-7ed5055d-cb39-4c1b-8acb-0eb1cefc4f8a.png)
![image](https://user-images.githubusercontent.com/24961188/190855613-6a586fd1-f2fb-4ba5-ae60-00b77615407a.png)


## 1.5 Conclusion: 
* Thus there are 447 closing high values out of 6399 close values which is about 7%. 
* Average wait is about 20 sessions. Which is somewhat wrong. 
* Max wait we have seen is 1406 Day which is about 46 month and that happened between 11-02-2000 to 18-12-2003 (Dot com bubble)
* Followed by 1094 days wait from 08-01-2008 to 05-11-2010 (Financial crisis) and then
* 1032 days wait from 05-11-2010 to 03-11-2013
* 90th percentile is ~18, 95th is ~48, 99th is ~529, 99.99 percentile is ~1267 (3 years, 6 months)
* So it make sense to hold the position for about 529 days (about 18 months) 
