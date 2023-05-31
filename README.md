# Illustrate data science lifecycle for selected case study (Product Recommendation)

Time series forecasting occurs when you make scientific predictions based on historical time stamped data. It involves building models through historical analysis and using them to make observations and drive future strategic decision-making. An important distinction in forecasting is that at the time of the work, the future outcome is completely unavailable and can only be estimated through careful analysis and evidence-based priors.
Time series allows you to analyze major patterns such as trends, seasonality, cyclicity, and irregularity. It is used for various applications such as stock market analysis, pattern recognition, earthquake prediction, economic forecasting, census analysis, etc.
Time series includes trend cycles and seasonality. 
•	Trend: An increase or decrease in data over a period of time is called a trend.
•	Seasonal: Oftentimes, seasonality is of a fixed and known frequency. For example, seasonal factors like the time of the year or the day of the week, a seasonal pattern occurs.
•	Cyclic: When a data exhibit fluctuates, a cycle occurs. But unlike seasonal, it is not of a fixed frequency.
Time series are used in statistics, signal processing, pattern recognition, econometrics, mathematical finance, weather forecasting, earthquake prediction, electroencephalography, control engineering, astronomy, communications engineering, and largely in any domain of applied science and engineering which involves temporal measurements.

About Project: I have taken the online sales data to check which is the most selled product.Also check along with that product which product is being selled. We can create a little helper function for our recommendation system to make it quick and easy to identify which products are associated with others. First, we use the corrwith() function to identify the Pearson correlation coefficient for each product with every other. When we run the get_recommendations() function we will pass in our item matrix dataframe containing each product and the number of times it co-occurred in a basket, as well as the column name for our target product. The recommender function will then calculate the Pearson correlation for the item and return the most correlated products, thus generating accurate product recs for us to display to the user on the product detail page. Also show the time series components using time series forecasting
Dataset Name: online_retail.csv
Steps to Analyze Time Series
•	Collecting the data and cleaning it - 
•	Preparing Visualization with respect to time vs key feature (PowerBi)
•	Observing the stationarity of the series (Components)
•	Developing charts to understand its nature.
•	Model building – MA (Moving Average)
•	Extracting insights from prediction 
Moving Average (MA):
Moving averages are calculated to identify the trend direction of a stock or to determine its support and resistance levels. It is a trend-following or lagging, indicator because it is based on past prices.
The longer the period for the moving average, the greater the lag. A 200-day moving average will have a much greater degree of lag than a 20-day MA because it contains prices for the past 200 days. 50-day and 200-day moving average figures are widely followed by investors and traders and are considered to be important trading signals.
Investors may choose different periods of varying lengths to calculate moving averages based on their trading objectives. Shorter moving averages are typically used for short-term trading, while longer-term moving averages are more suited for long-term investors.
While it is impossible to predict the future movement of a specific stock, using technical analysis and research can help make better predictions. A rising moving average indicates that the security is in an uptrend, while a declining moving average indicates that it is in a downtrend.
Similarly, upward momentum is confirmed with a bullish crossover, which occurs when a short-term moving average crosses above a longer-term moving average. Conversely, downward momentum is confirmed with a bearish crossover, which occurs when a short-term moving average crosses below a longer-term moving average.
Types of Moving Averages
1.	Simple Moving Average
A simple moving average (SMA), is calculated by taking the arithmetic mean of a given set of values over a specified period. A set of numbers, or prices of stocks, are added together and then divided by the number of prices in the set.
 
2.	Exponential Moving Average (EMA)
The exponential moving average gives more weight to recent prices in an attempt to make them more responsive to new information. To calculate an EMA, the simple moving average (SMA) over a particular period is calculated first.
Then calculate the multiplier for weighting the EMA, known as the "smoothing factor," which typically follows the formula: [2/(selected time period + 1)]. 
For a 20-day moving average, the multiplier would be [2/(20+1)]= 0.0952. The smoothing factor is combined with the previous EMA to arrive at the current value. The EMA thus gives a higher weighting to recent prices, while the SMA assigns an equal weighting to all values.
 
Visualisation of data with respect to time vs key feature
1.	Overview of visualisation
![image](https://github.com/Hinal0101/Product_Recommendation/assets/89678274/a4efcdad-2960-4178-b27a-98bfbd34bd1f)

2.	UnitPrice of year 2010 visualisation
![image](https://github.com/Hinal0101/Product_Recommendation/assets/89678274/02636d36-4943-4a9e-a0cb-afbc5df0f0f5)

3.	Unit price of year 2011 visualisation
![image](https://github.com/Hinal0101/Product_Recommendation/assets/89678274/373a2355-ffc3-4fd2-aedb-b3fa943c97e8)

4.	Unit price and quantity in October 2010
![image](https://github.com/Hinal0101/Product_Recommendation/assets/89678274/e7feba15-9c79-440e-9ece-5a4dc6fd0a76)

5.	Time series forecasting
a. 
![image](https://github.com/Hinal0101/Product_Recommendation/assets/89678274/9570baca-bcb6-4bee-ab80-66f94b639df0)

b.
![image](https://github.com/Hinal0101/Product_Recommendation/assets/89678274/b6577a5b-3108-4ba9-8f99-5ff7229243b4)

