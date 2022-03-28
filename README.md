
# Stock-Analysis
## VBA Challenge Write Up


## Overview

	The purpose of this analysis was to refactor or change the existing code created to analyze certain stocks. In refactoring, the goal was to decrease the amount of time it took to go through the code and obtain the different information outputs.  Refactoring the code would allow for larger data to be processed in a reasonable amount of time.

## Results

	After analyzing the different tickers in 2017 and 2018, 2017 was a much better year by its returns.  Most stocks where in the green indicating that the ending price was higher than the starting price.  2018 had a majority of the stocks in red meaning they closed at a lower value than where they started. 
	
<img width="1280" alt="VBA Stock Analysis 2017" src="https://user-images.githubusercontent.com/85581208/140005591-1eacd4a7-4a3f-4472-88d4-7fab37785530.png">


<img width="1280" alt="VBA 2018 Stock Analysis" src="https://user-images.githubusercontent.com/85581208/140005597-6211debd-5c92-491c-bfbf-a132dcb75502.png">

The execution time of the original code versus the refactored code did not seem like a big difference with only 12 stocks.  When applying a larger data set the time difference could be minutes or more depending on the data size.  Here is some of the original code.


<img width="1280" alt="VBA_Challenge_Original_Code" src="https://user-images.githubusercontent.com/85581208/140006225-3e5570f3-b615-4a14-abd0-68b0fa9f8438.png">

And here is the refactored code where instead of volume, tickerVolume was used along with tickerIndex to gather the data more efficiently.

<img width="1280" alt="VBA code" src="https://user-images.githubusercontent.com/85581208/140006282-de6a4841-6d44-4fb1-a648-67cdee9a9310.png">

Here are the execution times for 2017 and 2018 with the refactored code.

<img width="1280" alt="VBA_Challenge_2017" src="https://user-images.githubusercontent.com/85581208/140006764-35f3bb09-f7d3-459c-ab56-8180e64dd6ff.png">

<img width="1280" alt="VBA_challenge_2018" src="https://user-images.githubusercontent.com/85581208/140006485-49c64eb3-24d3-4d63-9697-45399f1d49d7.png">

There really was not a significant difference which was to be expected since both years ran through the same tickers.  With the original code, the run time was around 0.8 seconds.  7-8x slower.  Again not much of a measurable difference with such a small data set but if applied to 1000 different stocks the response time would be of value in using the refactored code.


## Summary
  In summary, refactoring has advantages and disadvantages.  One advantage is saving time in analyzing larger data sets.  If the code will be utilized over and over again, the time taken to refactor the code is worth the time ultimately saved in calculating the outputs from the data.  The disadvantages are the time taken to change the code.  Code can be finnicky and if it takes a lot of time to get it right to run more efficiently than it might not be worth the effort.  It also is a disadvantage, if the refactored code is not run on a big data set.  The time spent on refactoring the code may not be worth the time saved in the analyzation time.
