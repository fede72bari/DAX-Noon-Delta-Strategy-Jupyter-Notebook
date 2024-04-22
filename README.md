You can find full description of the results at the URL https://medium.com/@fede72bari/noon-delta-signal-analysis-on-dax-7fe40aa35916

-------------------------------------------------------------------------------------
Extract
-------------------------------------------------------------------------------------

<h1>Trading DAX: the Noon Delta Signal Analysis</h1>

<i>Copyright Federico Bari — April the 7th 2024 — fede72bari@gmail.com

Disclaimer: This document is published solely for coding and statistical analysis learning purposes. It is not intended to suggest, promote, or stimulate any trading strategy. Avoid using the results and remarks presented in this document for actual trading purposes, as it may contain bugs and mistakes. Moreover, future market conditions could differ from historical data, potentially leading to significant trading losses. Any suggestion, error/bug detection, and improvement is very welcome.</i>

It’s 4 months; 4 months that my friend Paolo warmly invites me for statistically testing and characterizing this strategy. Something he heard from somebody else; a gossip traveling the seas of trading forums and chats for years probably. I guess that Paolo now could be happy, but always possible undetected bugs in my code. More than 82% successful, simple strategy! Or … not?

<h2>Index</h2>
1.	Versions	<br>
2.	Preface	<br>
- Some expectations you may have on this publication	<br>
- What you won’t find for sure in this publication	<br>
- Prerequisites	<br>
- My expectations	<br>
- Code	<br>
- Time	<br>
- Uncorrelations with my job	<br>
3.	Strategy Description	<br>
4.	Libraries import	<br>
5.	Data sources	<br>
6.	Trading this strategy directly	<br>
- Preliminary analysis: is it worth to continue? A glance to statistics	<br>
- Back-testing the base strategy and some variations	<br>
- Basic trading strategy	<br>
- Stop Loss at 50 euro	<br>
- Stop loss at 93 euro	<br>
- Time to call Paolo	<br>
7.	Statistical Analysis	<br>
- After 12:00 maxes characterization	<br>
- Correlation between 9:00-12:00 min/max delta and after 12:00 min before max/max delta	<br>
- Min before after 12:00 max areas occurrences	<br>
- Number of 9:00-12:00 max threshold crosses after 12:00	<br>
- Distribution of delta between 9:00-12:00 and after 12:00 maxes	<br>
8.	Strategy Optimizations	<br>
9.	Implementing Statistical Suggestions for the DAX Noon Delta Signal	<br>
- Backtesting variable stop loss as a multiple of the take profit level	<br>
- Variation of the inner thresholds	<br>
- Time for metabolization	<br>
10.	Can Machine Learning improve this strategy?	<br>
- A preliminary look on clusterization <br>
- Attempts with classificators and regressors	<br>
- Mixing rule-based signals with ANN classificator ones	<br>
11.	Conclusions	<br>
12.	Annexes	<br>
- Annex A: full notebook	<br>
- Annex B: DAX Noon Delta indicator in Pine 5 code	<br>

