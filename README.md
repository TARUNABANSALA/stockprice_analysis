# stockprice_analysis
Stock-Market-Analysis-With-Python
Performing the Financial Analysis on Historic Stock Market Data such as calculating various risks, returns,etc.

ETL process:
Data exploration:
I did import Stock price data for Apple Inc. through API call to AlphaVantage.
Data is loaded in the form of Pandas Dataframe
Data Cleaning:
Check for Null values and cleaned the data accordinly

Visulaizations and Analysis:
Data Visualizations:
Apple stock prices were visualized 
(a) line chart of closing prices using Matplotlib:
This chart presents the closing prices of Apple stocks since 2000 till now. After analysis, it can be seen that the closing price were really high during two times one in 2012 to 2014 when it launched it ipad series and then in Corona-virus pandemic hit

(b) Basic Statistics:
Here's what each of these statistics indicates:
Mean Values: The mean (average) values for each attribute represent the central tendency of the data. For example, for the 'Open' attribute, the mean value is approximately 173.24, which means that the average opening price over the given time period is around $173.24.

Median Values: The median values for each attribute represent the middle value when the data is sorted. It's a measure of central tendency that is not affected by outliers. For the 'High' attribute, the median value is approximately 134.17, which indicates that half of the recorded high prices are above this value and half are below.

Standard Deviation Values: The standard deviation measures the dispersion or variability of the data points around the mean. A larger standard deviation indicates greater variability, while a smaller standard deviation indicates less variability. For the 'Low' attribute, the standard deviation is approximately 149.09, indicating that the low prices have a relatively high variability around the mean.

(c) Candlestick chart:
shows the open, high, low, and close prices for each trading day. This can provide insights into price movements within each day.A candlestick chart, also known as a Japanese candlestick chart, is a type of financial chart used to represent the price movements of an asset (such as a stock) over a specific time period, often a single trading day. Because its a larger data in terms of years the Candlestick chart was not that informative

(d) Correlation Heatmap:
Use a heatmap to visualize the correlation matrix between different stock attributes. Positive values indicate positive correlation, negative values indicate negative correlation, and values close to 0 indicate weak or no correlation. Here it can be said that high, low, close and open prices are all highly correlated with each other where as Volumes doesn't correlate with any of this. It shows negative correlation.

(e) Volume Chart:
Visualize the trading volume over time using a bar chart. This can help you identify periods of high trading activity. It shows the Volume activity of Apple stocks. The charts showed highest peaks of trading volume till now during the Pandemic hit which is kind of self explanatory.

(f) Moving Averages:
Moving Average (MA) Basics:
A moving average is a widely used technical indicator in financial analysis. It's calculated by averaging a set of data points over a specified period of time. In stock trading, the most common periods used are 50 days and 200 days.

200-Day Moving Average (200DMA) and Its Significance:
The 200-day moving average is a moving average calculated over the past 200 trading days. This time frame roughly corresponds to a year's worth of trading data (assuming a typical trading year of around 250 days). The 200DMA is often considered a key level in technical analysis due to its longer-term perspective.

Bullish and Bearish Trends:
Bullish Trend:
When the 50-day moving average (50DMA) of a stock price remains consistently higher than the 200DMA, it's generally interpreted as a bullish signal. This situation indicates that the stock's recent short-term performance (as indicated by the 50DMA) is stronger than its longer-term performance (as indicated by the 200DMA). This alignment suggests that the stock has been experiencing positive momentum and is likely in an upward trend. This can be observed in Apple stocks for high spikes in closing prices happened at 2000 to 2023. There are lot of spikes for high closing prices some of them are in 2012 to 2013 and 2014, Pandemic hits. 

Bearish Trend:
A crossover to the downside of the 200DMA is considered bearish. This means that the stock's 50DMA has dropped below the 200DMA. This situation suggests that the recent short-term performance of the stock is weakening compared to its longer-term performance. A downward crossover of the 200DMA may indicate a potential shift in sentiment and could signal that the stock's upward momentum is weakening, potentially leading to a downward trend.

Interpreting the Signal:

When the 50DMA is above the 200DMA, traders might interpret it as a sign of strength and potential buying opportunity.
When the 50DMA crosses below the 200DMA, it could indicate a weakening trend and prompt some traders to consider selling or taking a cautious approach.
It's important to note that while the 200DMA is a widely followed indicator, it's not foolproof. There can be false signals, and other factors, such as company news, economic events, and market sentiment, should also be considered in trading decisions.

(g) Volatility Visualization:
Plot the range between high and low prices over time to visualize stock price volatility.This example calculates the price range (volatility) between high and low prices for each date and then plots the price range over time. The y-axis represents the price range, and the x-axis represents the dates. This allows you to visually observe periods of high and low volatility in the stock's price movements. The highest volatility in price range of 60 was recorded at 2010-05-06
Volatility Statistics:
Average Volatility: 3.98: The average volatility of 3.98 indicates that, on average, the difference between the high and low prices of Apple stock over the analyzed period is around 3.98 units (currency, points, etc.). This value provides a general sense of the stock's price range variability. An average volatility of 3.98 might suggest that the stock experiences moderate price fluctuations on a regular basis.

Median Volatility: 2.74: The median volatility of 2.74 is lower than the average volatility. The median represents the middle value of the price range data when ordered from smallest to largest. The fact that the median is lower than the mean (average) suggests that there might be some extreme price range values (outliers) that are influencing the mean to be higher. The median is less sensitive to outliers, making it a useful measure when data has extreme values.

Standard Deviation of Volatility: 3.89: The standard deviation of 3.89 quantifies the spread or dispersion of the price range values around the mean volatility. A higher standard deviation indicates greater variability in the price range, which suggests that the stock's price can experience significant fluctuations from day to day. The standard deviation being close to the average volatility implies that there might not be extremely large deviations from the average, but rather a more consistent spread of volatility values.

Based on these measures, it appears that the stock experiences moderate volatility, with the majority of price range values clustering around the average volatility. The higher standard deviation suggests that there are some days with larger price fluctuations, but they are not too far from the norm.

(h) Performance Metrics:
Apple Stock Daily Returns
Apple Stock Cumulative Returns

(i) Time series analysis:
    (1) Autocorrelation plot for the closing prices:
    On the graph, there is a vertical line (a "spike") corresponding to each lag. The height of each spike shows the value of the autocorrelation function for the lag.The autocorrelation with lag zero always equals 1, because this represents the autocorrelation between each term and itself. Price and price with lag zero are the same variable.Each spike that rises above or falls below the dashed lines is considered to be statistically significant. This means the spike has a value that is significantly different from zero. If a spike is significantly different from zero, that is evidence of autocorrelation. A spike that's close to zero is evidence against autocorrelation.
    In this example, the spikes are statistically significant for lags up to 24. This means that the Apple stock prices are highly correlated with each other. In other words, when the price of Apple stock rises, it tends to continue rising. When the price of Apple stock falls, it tends to continue falling. This figure illustrates this.
    Autocorrelation plot for the daily returns:
    This figure shows an autocorrelation plot for the daily returns to Apple stock from 2000 to 2023.The autocorrelation plot for daily returns to Apple stock shows that most of the spikes are not statistically significant. This indicates that the returns are not highly correlated, as shown here. The graph shows that except for one major downturn, the returns to Apple stock between 2000 and 2023 do not show any particular pattern — they tend to fluctuate randomly around zero. This means that the returns are largely independent of each other. You can use an autocorrelation plot to determine whether the elements of a time series are random (that is, unrelated to each other). This is important, because many statistical tests involving time series are based on this assumption.
    (2) Seasonal Decomposition: