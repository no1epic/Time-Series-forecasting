# Stock Analysis: Amazon & Netflix

## Overview
This project provides a comprehensive analysis of Amazon and Netflix stock trends over a one-year period (252 trading days). The analysis incorporates historical stock assessment, short-term and long-term forecasting, and regression modeling to uncover insights into the stock behavior and predict future trends.

## Objectives
The primary goals of this project are:
1. Perform short-term and long-term stock price forecasting using exponential smoothing and weighted moving averages.
2. Develop regression models to analyze trends and evaluate residuals for independence and normal distribution.
3. Compare the effectiveness of different forecasting techniques.

## Tools and Technologies
- **Python:** Core programming language for data processing and modeling.
- **Excel:** For managing and analyzing stock data.
- **Statistical Tests:** Mean Absolute Percentage Error (MAPE), Mean Absolute Percentage Deviation (MAPD), Chi-Square test.
- **Visualization Libraries:** Matplotlib for data visualization.

## Process
### 1. Data Preparation
- Historical stock prices for Amazon and Netflix were analyzed for 252 trading days.
- The data was visualized to understand seasonality and volatility.

### 2. Short-Term Forecasting
- **Exponential Smoothing:**
  - Alpha values (0.20, 0.40, 0.60, and 0.80) were tested for both stocks.
  - MAPE and MAPD were calculated to evaluate forecast accuracy.
  - Alpha = 0.80 yielded the lowest MAPE for both stocks, providing the most accurate short-term forecasts.

### 3. Long-Term Forecasting
- A three-period weighted moving average was applied.
- Weights of 0.5, 0.3, and 0.2 were used to forecast trends.
- Amazon showed lower forecasting errors compared to Netflix, making it the preferred model for long-term analysis.

### 4. Regression Modeling
- Regression analysis was performed to identify trends in stock prices.
- Residuals were evaluated for independence, homoscedasticity, and normal distribution using Chi-Square tests.
- Both stocks exhibited non-normal distribution and dependent residuals, indicating limitations in the regression model.

## Key Findings
- **Short-Term Insights:**
  - Exponential smoothing provided the most accurate forecasts for both stocks.
  - Higher alpha values placed more emphasis on recent data, improving short-term accuracy.

- **Long-Term Insights:**
  - Amazon's trend analysis exhibited lower errors than Netflix, suggesting better predictive reliability.

- **Regression Analysis:**
  - Residuals were not normally distributed, confirmed by Chi-Square test results.
  - The regression model had the highest error rate among all methods.

## Portfolio Recommendation
Based on the analysis:
- Allocate 60% investment to Amazon and 40% to Netflix, leveraging Amazon's lower forecasting error and consistent trends.

## Challenges
- Handling residual dependencies and non-normality in regression modeling.
- Balancing accuracy and complexity in long-term forecasting methods.

## Future Enhancements
- Incorporate advanced forecasting models like ARIMA or machine learning algorithms.
- Expand the analysis period to include multiple years.
- Factor in external market variables to improve prediction accuracy.

## References
1. [Forecasting Statistical Details](https://www.ibm.com/docs/en/cognos-analytics/11.1.0?topic=forecasting-statistical-details)
2. [Mean Average Percentage Error](https://support.numxl.com/hc/en-us/articles/215959443-MAPE-MeanAbsolutePercentageError#:%7E:text=MAPE%20is%20also%20referred%20to%20as%20MAPD)
3. [Time Series and Business Forecasting](http://home.ubalt.edu/ntsbarsh/stat-data/forecast.htm#rhowma)
4. [Residual Analysis](https://web.ma.utexas.edu/users/mks/statmistakes/modelcheckingplots.html#:%7E:text=Rule%20of%20Thumb%3A%20To%20check,random%20suggests%20lack%20of%20independence)

## Author
**Sahil Gawande**
