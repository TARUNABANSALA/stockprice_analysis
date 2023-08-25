# stockprice_analysis
Stock-Market-Analysis-With-Python
Performing the Financial Analysis on Historic Stock Market Data such as calculating various risks, returns,etc.

Understanding Stock Analysis
Stock analysis is a method for investors and traders to make buying and selling decisions. By studying and evaluating past and current data, investors and traders attempt to gain an edge in the markets by making informed decisions.

Technical Analysis
This analysis focuses on the study of past and present price action to predict the probability of future price movements. It will analyze the financial market as a whole and are primarily concerned with price and volume, as well as the demand and supply factors that move the market.
Charts are a key tool for technical analysts as they show a graphical illustration of a stock’s trend within a stated time period. For example, using a chart, a technical analyst may mark certain areas as a support or resistance level. The support levels are marked by previous lows below the current trading price, and the resistance markers are placed at previous highs above the current market price of the stock. A break below the support level would indicate a bearish trend to the stock analyst, while a break above the resistance level would take on a bullish outlook.

Standard Deviation : Standard deviation is a number used to tell how measurements for a group are spread out from the average (mean), or expected value i.e, what is the percentage that inverstors will be surprised by the result.

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
This chart presents the closing prices of Apple stocks since its launched till now. After analysis, it can be seen that the closing price were really high during two times one in 2012 to 2014 when it launched it ipad series and then in Corona-virus pandemic hit

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
A moving average is a commonly used technical indicator that helps smooth out price data over a specified period of time. Plot moving averages (e.g., 50-day and 200-day moving averages) along with the actual stock prices to observe trends more clearly.The different lines on the plot allow you to observe trends more clearly and identify potential crossovers or patterns.

Moving averages can help traders and investors in several ways:

Trend Identification: Moving averages are often used to identify the direction of the trend. If the stock's price is consistently above its moving average, it could indicate an uptrend, and vice versa for a downtrend.

Support and Resistance Levels: Moving averages can act as dynamic support and resistance levels. In an uptrend, the moving average might act as a support level, and in a downtrend, as a resistance level.

Crossovers: When a shorter-term moving average crosses above a longer-term moving average, it's often considered a bullish signal, suggesting potential upward momentum. Conversely, a crossover where the shorter-term moving average crosses below the longer-term one can be seen as a bearish signal.

Reversal Indicators: Changes in the relationship between price and moving averages can indicate potential trend reversals. For instance, if a stock that has been trending downward crosses above its moving average, it might signal a reversal.

The 200-day moving average is considered especially significant in stock trading. As long as the 50-day moving average of a stock price remains above the 200-day moving average, the stock is generally thought to be in a bullish trend. A crossover to the downside of the 200-day moving average is interpreted as bearish.

(g) Volatility Visualization:
(h) Performance Metrics:
(i) Time series analysis:
    (1) Autocorrelation:
    (2) Seasonal Decomposition: