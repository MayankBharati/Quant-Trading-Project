![222331629-1251660d-9ad8-4545-b970-016715b609f8](https://github.com/MayankBharati/Quant-Trading-Project/assets/75744167/9540d5fc-6fa5-4b58-90ce-837eb5da4c4d)# Quantitative Analysis Using Golden Cross and EMA

## Overview

In this GitHub project, we explore a quantitative trading strategy based on the "Golden Cross" and "Death Cross" concepts, using Exponential Moving Averages (EMA). This strategy has gained significant attention in recent years and is widely employed by traders aiming to achieve substantial returns. Our project implements and evaluates this trading strategy, comparing its performance with a traditional buy-and-hold approach across equity, forex, and cryptocurrency markets.

## Trading Strategy

Our trading strategy relies on the principles of moving averages, specifically the Simple Moving Average (SMA) and the Exponential Moving Average (EMA). These moving averages are crucial technical indicators used to identify trends and inform trading decisions. The Golden Cross, a bullish indicator, occurs when a short-term moving average crosses above a long-term moving average, while the Death Cross, a bearish indicator, happens when the short-term moving average crosses below the long-term moving average. By using these crosses, we aim to pinpoint optimal entry and exit points in the market.

## Datasets

We apply this strategy to three distinct asset classes: stocks, currencies, and cryptocurrencies. Our data is sourced automatically through APIs, with stock and currency data collected from Yahoo Finance and cryptocurrency data gathered from Binance. The data spans a ten-year period, with daily intervals, and is meticulously cleaned to remove holidays, non-trading days, and anomalies. Notably, the stock dataset includes approximately 2,500 stocks, the currency dataset features the top 500 pairs based on data availability, and the cryptocurrency dataset comprises data from Binance, taking into account delisted tokens.

## Methodology

Our approach involves calculating short and long EMAs based on user-defined input periods. The strategy triggers long positions when a Golden Cross (sign change from -1 to +1) is detected and short positions when a Death Cross (sign change from +1 to -1) occurs. We record the dates of these positions and calculate returns during these periods, comparing them against a buy-and-hold strategy. We perform this process for various combinations of EMA, SMA, and price, selecting the strategy with the best performance.

## Performance

Performance results vary across asset classes:

- **Equity**: This is by far the Best Trading Performance. Achieves a total return of 189.2% from May 2012 to May 2022, with an annualized return of 11.2%. A short-term trend and 200-day EMA are utilized for this model, and long positions are closed on Death Cross signals.
- ![222331544-15b19db9-1e9c-4f4f-abca-46c8d42dbd9b](https://github.com/MayankBharati/Quant-Trading-Project/assets/75744167/25d84cdb-5741-48d9-a94e-634630934090)
- ![222331544-15b19db9-1e9c-4f4f-abca-46c8d42dbd9b](https://github.com/MayankBharati/Quant-Trading-Project/assets/75744167/7a5ff0b2-5b66-46da-9838-92497c56afe2)





- **Forex**: This is by far the Worst Trading Performance  Records the worst returns over the same period, resulting in total returns of -61.3%. The strategy involves using the 50-day and 200-day EMA. Long positions are closed on Death Cross signals, and short positions are taken.
- ![222331629-1251660d-9ad8-4545-b970-016715b609f8](https://github.com/MayankBharati/Quant-Trading-Project/assets/75744167/a18bc6df-20e6-42ec-b936-b2ac468d3bd4)


- **Cryptocurrency**: This is by far an Average Trading Performance  Demonstrates an average performance, with median returns of 40.91% from July 2017 to June 2022. The strategy uses a short-term trend and a 200-day EMA. Due to high cryptocurrency volatility, swift actions are essential to mitigate drawdown.
- ![222331665-42f80ee1-e2b2-4413-9e70-9812b4be8142](https://github.com/MayankBharati/Quant-Trading-Project/assets/75744167/dc9a9684-b203-4388-97d0-13fb03e9fb21)


## Key Takeaways and Conclusion

Our project provides valuable insights into the potential of the Golden Cross and EMA trading strategy across various asset classes. It underscores the need for ongoing refinement and adaptability in the ever-changing world of financial markets. While the strategy shows promise, there are limitations that require further improvements, such as confirming signals across multiple periods, diversification, and the introduction of threshold returns and stop-loss mechanisms.

Feel free to explore the code and data in this repository to gain a deeper understanding of our analysis and to contribute to the ongoing development and optimization of this trading strategy. Your contributions are welcome as we continue to refine this strategy for better performance and broader applicability.
