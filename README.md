# Zillow-Data-Modeling
This project aims to determine the top 5 best zip codes for real estate investment using Zillow data. The analysis includes data preprocessing, ARIMA model development, evaluation, and recommendations for investment strategies.

# Table of Contents
Installation

Usage

Features

# Installation

## Clone the repository

git clone https://github.com/your-username/real-estate-investment-analysis.git
cd real-estate-investment-analysis

# Usage
To run the analysis, open the Jupyter notebook and execute the cells step-by-step:

## Start Jupyter Notebook:

## Open the notebook:
Open Phase 4 Group 9.ipynb in the Jupyter interface.

## Run the cells:
Execute the cells in the notebook to preprocess the data, build and evaluate the ARIMA model, and view the recommendations.

# Features
## Data Preprocessing: 
Handling missing values, dropping columns, filling columns in preparation of modeling.

## EDA and Visualizations: 
Univariate Analysis, Bivariate Analysis, Handling Outliers.

## ARIMA Model Development: 
Stationarity check and Differencing, Building an ARIMA model for time series forecasting of real estate prices.

## Evaluation: 
Model Summary The SARIMAX model was applied to the real estate price data, and the results are summarized below:

Model: ARIMA(1, 2, 1)
Number of Observations: 265
Log Likelihood: -1829.066
AIC (Akaike Information Criterion): 3664.131
BIC (Bayesian Information Criterion): 3674.848
HQIC (Hannan-Quinn Information Criterion): 3668.438
Parameter Estimates

AR(1) Coefficient: -0.3828 (std err: 0.615, z: -0.622, p: 0.534)
MA(1) Coefficient: 0.3319 (std err: 0.621, z: 0.534, p: 0.593)
Sigma^2 (Variance of the error term): 6.332e+04 (std err: 1490.737, z: 42.477, p: 0.000)
Diagnostic Tests

Ljung-Box (L1) Test (Q): 5.89 (Prob(Q): 0.02)
Jarque-Bera (JB) Test: 10222.20 (Prob(JB): 0.00)
Heteroskedasticity (H) Test: 4.53 (Prob(H) (two-sided): 0.00)
Skewness: -2.10
Kurtosis: 33.25
Model Fit:

The model is an ARIMA(1, 2, 1), indicating that it includes one autoregressive term, two differencing steps, and one moving average term.
The low p-values for the Ljung-Box and Jarque-Bera tests indicate that there are some issues with residual autocorrelation and non-normality of residuals, respectively. This may suggest that the model could be improved.
Parameter Significance:

The p-values for the AR(1) and MA(1) coefficients are 0.534 and 0.593, respectively, suggesting that these parameters are not statistically significant. This could imply that the model might not be capturing the underlying patterns effectively.
Variance:

The sigma^2 value is high, indicating significant variability in the data, which is to be expected in real estate prices.
Diagnostics:

Ljung-Box Test: The p-value of 0.02 suggests that there may be some autocorrelation in the residuals, indicating that the model does not fully capture the time series structure.
Jarque-Bera Test: The high JB statistic with a p-value of 0.00 indicates that the residuals are not normally distributed, which might affect forecast accuracy.
Heteroskedasticity Test: The significant p-value suggests heteroskedasticity in the residuals, meaning that the variance of the residuals changes over time.
Skewness and Kurtosis: The negative skewness and high kurtosis indicate that the residuals are not normally distributed and have heavy tails.
Conclusion
Investment Potential:

The top 5 identified zip codes show high potential for real estate investment based on historical price trends and forecasted growth. These zip codes balance high profit potential with manageable risk levels, making them attractive for investment.

Risk Assessment:

Volatility analysis suggests that while some high-value areas are riskier, they also offer higher returns. More stable areas provide safer investment options with moderate returns.

## Investment Recommendations: 
Diversified Investment:

Invest in a diversified portfolio that includes both high-growth, high-volatility areas and stable, moderate-growth areas.
This strategy will balance the potential for high returns with risk management.
Long-Term Investment:

Focus on long-term investment strategies in areas with strong upward trends and stable growth.
Short-term investments can be considered in high-volatility areas with careful monitoring of market conditions.
Continuous Monitoring:

Continuously monitor market conditions and economic indicators that could impact the real estate market.
Adjust investment strategies based on new data and forecasts to optimize returns and manage risks
