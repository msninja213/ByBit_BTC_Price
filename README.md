This code uses the ccxt library to access the exchange ByBit to get Bitcoin data. 

We collected OHLCV data on Bitcoin every 5 minutes over the past 90 days. We created two data frames, one for BTC price over the weekdays vs weekend for easy analysis. 

We began by plotting the price of BTC over the weekdays and weekend, then went on to analyze difference in volume. It's evident that the weekdays consistently have a higher trading volume than the weekend, though there are a few large spikes over the weekend that could be chalked up to current events. 

From here, we decided to analyze the percent change between daily close and open prices for the weekdays vs the weekend, and found that the weekdays had a higher percent change. This makes sense because there is an increase in trading volume over the weekdays. We then decided to see what the weekly returns would be if we bought BTC on Monday and sold it on Friday vs buying it Saturday and selling it Sunday. Once again, the weekday returns were greater. 

From here, we were interested in seeing if certain trading days were better than other days by graphing the cumulative return of each day of the week. We found that Wednesday had the highest cumulative return while Thursday had the lowest. This prompted us to wonder, to what extent could we justify trading on the weekday vs the weekend? 

This led us to completing a max drawdown analysis, where we graphed the cumulative returns and drawdown for the weekday vs weekend. We also calculated the max drawdown value and Calmar ratio. We found that the Calmar ratio was higher for the weekend vs weekday, showing that profit has a higher chance of exceeding the max drawdown. However, annualized returns are much lower over the weekend. 
