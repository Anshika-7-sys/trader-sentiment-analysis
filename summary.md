# 📊 Executive Summary

## Methodology
The dataset was first cleaned and standardized, including timestamp correction, column normalization, and aggregation at the account-date level. Trading activity was merged with sentiment classifications to create a unified analytical dataset.
Feature engineering included:
* Average trade size (exposure proxy)
* Trade frequency (activity intensity)
* Loss ratio (risk behavior indicator)
* Next-day profitability target variable
A Random Forest classifier was developed to predict next-day profitability using behavioral and sentiment features. Model performance was evaluated using train-test split validation.
To complement supervised learning, K-Means clustering was applied at the trader level to identify behavioral segments based on profitability, trade size, activity level, and risk exposure.
## Key Insights
1. Behavioral metrics dominate predictive performance.
   Feature importance analysis shows that trade size (~55%) and trade frequency (~38%) are the strongest drivers of next-day profitability.
2. Sentiment has incremental influence.
   While sentiment regimes (Fear, Greed, etc.) affect behavior patterns in exploratory analysis, they contribute less to direct predictive power compared to trader-specific behavior.
3. Model performance is meaningful.
   The predictive model achieved 63% accuracy, demonstrating that short-term profitability exhibits partially learnable behavioral structure.
4. Distinct trader archetypes exist.
   Clustering revealed three primary segments:
   * Conservative low-risk traders
   * Active consistent traders
   * High-risk high-reward traders
     Higher profitability clusters also exhibited higher exposure and volatility.
## Strategic Recommendations
* Risk management systems should prioritize monitoring trade size and trading intensity.
* Behavioral profiling is more effective than relying solely on sentiment indicators.
* Trader segmentation can enable personalized risk controls and performance monitoring.
* High-exposure traders require volatility-aware oversight despite higher average returns.
