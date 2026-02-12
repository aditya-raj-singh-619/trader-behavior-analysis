# trader-behavior-analysis
Data-driven analysis of trader performance vs Bitcoin market sentiment (Fear/Greed), including behavioral segmentation, strategy insights, and predictive modeling.

Trader Behavior vs Market Sentiment Analysis:
Objective: Analyze how Bitcoin market sentiment (Fear vs Greed) influences trader behavior and performance on Hyperliquid.
The goal is to uncover actionable insights that can inform smarter trading strategies.

Dataset Overview:
1. Historical Trader Data:
   1.Trade-level execution data
   2.211,224 rows
   3.Includes: PnL, trade size, timestamp, side, fees, etc.

2.Fear & Greed Index: 
   1.Daily market sentiment classification
   2.2,644 rows
   3.Sentiment categories: Fear, Greed (and Neutral/Extreme variants)


Methodology:
   1.Data Preparation
       1.Checked for missing values and duplicates (none found)
       2.Converted timestamps to daily level
       3.Aligned trader data with sentiment data by date

   2.Feature Engineering
   Created key metrics:
       1.Daily PnL per trader
       2.Win rate
       3.Average trade size
       4.Trade frequency
       5.Long/Short ratio
       6.Exposure proxy (avg position size)

   3.Analysis
       1.Compared Fear vs Greed performance
       2.Analyzed behavioral changes under different sentiment regimes
       3.Identified trader segments:
              1.High vs Low exposure
              2.Frequent vs Infrequent traders
              3.Consistent vs Inconsistent traders

   4.Bonus
       1.Built a simple predictive model for profitability
       2.Applied KMeans clustering to identify behavioral archetypes
