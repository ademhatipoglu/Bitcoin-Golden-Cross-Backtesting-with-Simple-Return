Buy Golden Cross Trading Strategy for Bitcoin

This project implements a trading strategy for Bitcoin (BTC-USD) using the quantmod and PerformanceAnalytics libraries in the R programming language. The strategy is based on the concept of a "Golden Cross," which involves comparing the exponential moving averages (EMA) of different periods and generating buy (1) or hold (0) signals accordingly.

To run this project, please follow these steps:

Install the required libraries: quantmod and PerformanceAnalytics. You can install them using the following commands in your R console:

arduino
Copy code
install.packages("quantmod")
install.packages("PerformanceAnalytics")
Open the R script file containing the code.

Adjust the date range for historical data by modifying the 'from' and 'to' parameters in the getSymbols() function. The default range is set from January 1, 2019, to the current date.

Set the values for the variables 'n', 'delta', 'S', and 'L' based on your trading strategy preferences:

'n' represents the number of periods to calculate the RSI.
'delta' is the threshold value for the Golden Cross signal.
'S' represents the short period for the EMA calculation.
'L' represents the long period for the EMA calculation.
Execute the script to load the BTC-USD historical data, calculate the EMA, RSI, and generate the buy signals based on the Golden Cross strategy.

The resulting performance of the strategy will be plotted using the PerformanceAnalytics library.

Please note the following:

This script assumes you have an active internet connection to download the historical data for BTC-USD.
The Golden Cross strategy implemented in this project compares the EMA values and generates a buy signal (1) when the short-term EMA is greater than the long-term EMA by a threshold (delta), and a hold signal (0) otherwise.
The performance of the strategy is evaluated by multiplying the daily returns of BTC-USD by the trading signals.
For any further questions or assistance, please reach out to ademhat10@gmail.com
