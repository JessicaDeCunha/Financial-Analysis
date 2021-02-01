# Quantitiative Financial Analysis Using Pandas

## Background


Quantitative analysis techniques with Python and Pandas, to determine which portfolio is performing the best across many areas: volatility, returns, risk, and Sharpe ratios.

I have created a tool (an analysis notebook) that analyzes and visualizes the major metrics of the portfolios across all of these areas, and determine which portfolio outperformed the others. I have used the historical daily returns of several portfolios: some from the firm's algorithmic portfolios, some that represent the portfolios of famous "whale" investors like Warren Buffett, and some from the big hedge and mutual funds. I then used this analysis to create a custom portfolio of stocks and compared its performance to that of the other portfolios, as well as the larger market (S&P 500).


## Instructions

File: Whale Analysis Starter Code

Use Pandas to read in each of the CSV files as a DataFrame. Be sure to convert the dates to a DateTimeIndex.


Detect and remove null values.


Remove dollar signs from the numeric values and convert the data types as needed.


The whale portfolios and algorithmic portfolio CSV files contain daily returns, but the S&P 500 CSV file contains closing prices. Convert the S&P 500 closing prices to daily returns.


Join Whale Returns, Algorithmic Returns, and the S&P 500 Returns into a single DataFrame with columns for each portfolio's returns.




Conduct Quantitative Analysis
Analyze the data to see if any of the portfolios outperform the stock market (i.e., the S&P 500).

Performance Analysis

Calculate and plot cumulative returns. Does any portfolio outperform the S&P 500?


Risk Analysis


Create a box plot for each of the returns. Which box has the largest spread? Which has the smallest spread?


Calculate the standard deviation for each portfolio. Which portfolios are riskier than the S&P 500?


Calculate the annualized standard deviation (252 trading days).



Rolling Statistics


Plot the rolling standard deviation of the various portfolios along with the rolling standard deviation of the S&P 500 using a 21 day rolling window. Does the risk increase for each of the portfolios at the same time risk increases in the S&P?


Construct a correlation table for the algorithmic, whale, and S&P 500 returns. Which returns most closely mimic the S&P?


Choose one portfolio and plot a rolling beta between that portfolio's returns and S&P 500 returns over a 60 day period. Does the portfolio seem sensitive to movements in the S&P 500?


BONUS - Additional 5 points An alternative way to calculate a rolling window is to take the exponentially weighted moving average. This is like a moving window average, but it assigns greater importance to more recent observations. Try calculating the ewm with a 21 day half-life.



Plot Sharpe Ratios
Investment managers and their institutional investors look at the return-to-risk ratio, not just the returns. (After all, if you have two portfolios that each offer a 10% return, yet one is lower risk, you would invest in the lower-risk portfolio, right?)


Using the daily returns, calculate and visualize the Sharpe ratios using a bar plot.


Determine whether the algorithmic strategies outperform both the market (S&P 500) and the whales portfolios.



Create Custom Portfolio
Harold is ecstatic that you were able to help him prove that the algorithmic trading portfolios are doing so well compared to the market and whales' portfolios. However, now you are wondering whether you can choose your own portfolio that performs just as well as the algorithmic portfolios. Investigate by doing the following:


Visit Google Sheets and use the in-built Google Finance function to choose 3-5 stocks for your own portfolio.


Download the data as CSV files and calculate the portfolio returns.


Calculate the returns for each stock.


Using those returns, calculate the weighted returns for your entire portfolio assuming an equal amount invested for each stock.


Add your portfolio returns to the DataFrame with the other portfolios and rerun the analysis. How does your portfolio fair?



Your analysis should include the following:

Using all portfolios:

The annualized standard deviation (252 trading days) for all portfolios.
The plotted rolling standard deviation using a 21 trading day window for all portfolios.
The calculated annualized Sharpe Ratios and the accompanying bar plot visualization.
A correlation table.


Using your custom portfolio and one other of your choosing:

The plotted beta. . How does your portfolio fair?





Resources
Pandas API Docs


Hints


After reading each CSV file, don't forget to sort each DataFrame in ascending order by the Date using sort_index. This is especially important when working with time series data as we want to make sure Date indexes go from earliest to latest.


The Pandas functions used in class this week will be useful for this assignment.


Be sure to use head() or tail() when you want to look at your data but don't want to print to a large DataFrame.




Submission


Create a Jupyter Notebook containing your data preparation, analysis, and visualizations. Put your analysis and answers to the assignment questions in raw text (markdown) cells in the report.


Submit your notebook to a new GitHub repository.


Add the URL of your GitHub repository to your Assignment when submitting via Bootcamp Spot.


