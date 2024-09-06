This repository contains the files of a data analysis project to test the profitability of an Ichimoku-based stock trading algorithm.
(*For more on [Ichimoku](https://en.wikipedia.org/wiki/Ichimoku_Kink%C5%8D_Hy%C5%8D) specifically and the admittedly questionable efficacy
of [technical indicators](https://en.wikipedia.org/wiki/Technical_analysis) generally, see their Wikipedia pages.*)
My intention is to provide working Python code that can be modified/expanded for much more serious/rigorous applications
(more sophisticated algorithms, different instruments etc.) and to test an interesting strategy.

The [data](data) folder contains historical (2020—2023) daily OHLC data CSVs, downloaded from Yahoo Finance, for all 30 DJIA stocks.
After reading and cleaning, relevant indicator lines are calculated, the strategy is simulated and the returns are printed.
Keeping in mind many simplifying assumptions (e.g., trades execute immediately at each day's close and its price),
the model earns, on average, a 20% yearly profit (using exponential growth) while having good risk mitigation through diversification.
