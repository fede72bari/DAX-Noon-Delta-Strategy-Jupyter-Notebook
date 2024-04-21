You can find full description of the results at the URl https://medium.com/@fede72bari/noon-delta-signal-analysis-on-dax-7fe40aa35916

-------------------------------------------------------------------------------------
Extract
-------------------------------------------------------------------------------------

<h1>Noon Delta Signal Analysis on DAX</h1>

<i>Copyright Federico Bari — April the 7th 2024 — fede72bari@gmail.com

Disclaimer: This document is published solely for coding and statistical analysis learning purposes. It is not intended to suggest, promote, or stimulate any trading strategy. Avoid using the results and remarks presented in this document for actual trading purposes, as it may contain bugs and mistakes. Moreover, future market conditions could differ from historical data, potentially leading to significant trading losses. Any suggestion, error/bug detection, and improvement is very welcome.</i>

It’s 4 months; 4 months that my friend Paolo warmly invites me for statistically testing and characterizing this strategy. Something he heard from somebody else; a gossip traveling the seas of trading forums and chats for years probably. I guess that Paolo now could be happy, but always possible undetected bugs in my code. More than 82% successful, simple strategy! Or … not?

<h2>Index<\h2>
1.	Versions	4
2.	Preface	5
Some expectations you may have on this publication	5
What you won’t find for sure in this publication	5
Prerequisites	5
My expectations	5
Code	6
Time	6
Uncorrelations with my job	6
3.	Strategy Description	7
4.	Libraries import	8
5.	Data sources	9
6.	Trading this strategy directly	11
Preliminary analysis: is it worth to continue? A glance to statistics	11
Back-testing the base strategy and some variations	14
Basic trading strategy	14
Stop Loss at 50 euro	18
Stop loss at 93 euro	21
Time to call Paolo	23
7.	Statistical Analysis	25
After 12:00 maxes characterization	25
Correlation between 9:00-12:00 min/max delta and after 12:00 min before max/max delta	27
Min before after 12:00 max areas occurrences	29
Number of 9:00-12:00 max threshold crosses after 12:00	29
Distribution of delta between 9:00-12:00 and after 12:00 maxes	30
8.	Strategy Optimizations	32
9.	Implementing Statistical Suggestions for the DAX Noon Delta Signal	35
Backtesting variable stop loss as a multiple of the take profit level	35
Variation of the inner thresholds	37
Time for metabolization	44
10.	Can Machine Learning improve this strategy?	45
A preliminary look on clusterization	45
Attempts with classificators and regressors	49
Mixing rule-based signals with ANN classificator ones	51
11.	Conclusions	65
12.	Annexes	67
Annex A: full notebook	67
Annex B: DAX Noon Delta indicator in Pine 5 code	68

