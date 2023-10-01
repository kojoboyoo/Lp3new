# Store Sales Forecasting using Time Series Analysis
## Introduction
Welcome to the Store Sales Forecasting project!
In this intriguing project, we delve into the realm of time series analysis to predict store sales for Corporation Favorita, a major grocery retailer in Ecuador. The goal is to leverage historical sales data, along with supplementary information like promotions, oil prices, holidays, and store metadata, to construct a robust predictive model. By harnessing the power of data insights, we aim to provide accurate forecasts that empower businesses to enhance decision-making, optimize resources, and ultimately boost their bottom line. Join us on this journey as we explore, analyze, and model the intricate sales dynamics to unlock valuable insights and guide strategic choices.
## Libraries installations
* Pandas, NumPy for data manipulation and cleaning.
* Matplotlib, Seaborn, Plotly for data visualization.
* Statsmodels, SciPy for statistical analysis.
* Scikit-learn for feature engineering and machine learning.
* ARIMA,LinearRegression,DecisionTreeRegressor,Xgboost for modeling
* Pyodbc, dotenv for database access. 
## Datasets
* Sales records
* Store metadata: includes city, state, type, and cluster.
* Transaction data
* Oil prices
* Holiday events
* Train and Test datasets 
## Methods and Techniques
* KPSS for testing stationarity 
* Differencing to make dataset stationary
* Autocorrelation for autocorrelation testing 

### Data Preparation and Exploration
Prior to diving into modeling, we meticulously prepared and explored the data. This involved cleaning datasets, handling missing values, and transforming variables for a cohesive analysis. Through in-depth exploration, we gained valuable insights into sales patterns, identifying outliers and trends crucial for modeling accuracy.

### Hypothesis Analysis and Visualization
Utilizing statistical techniques and visualization tools, we formulated hypotheses about the relationships between external factors like promotions, oil prices, and holidays, and store sales. Visualization aided in understanding complex trends, guiding our feature engineering strategies.

### Feature Engineering
Feature engineering played a crucial role in bolstering our models. By transforming raw data into meaningful features, we significantly improved the accuracy of our predictions. Techniques like incorporating lagged sales, rolling mean, rolling standard deviation, and considering the day of the week were pivotal. These transformed variables were instrumental in capturing the nuanced and complex patterns within the sales data, enabling our models to make more precise forecasts. 

### Time Series Decomposition
Time series decomposition allowed us to break down sales data into trend, seasonal, and residual components. This decomposition provided a clearer understanding of underlying patterns, aiding in model selection and evaluation
### Model Building
1. Models used
* ARIMA: Leveraged for its ability to capture time series patterns and seasonality.
* Linear Regression: Applied for baseline predictions, offering insights into linear relationships between variables.
* Decision Tree Regressor: Beneficial for capturing nonlinear relationships, especially in complex datasets.
* XGBoost: A powerful ensemble learning method, chosen for its robustness and accuracy in handling diverse features.
  
2.  Model Evaluation
Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE) and Root Mean Squared Logarithmic Error (RMSLE): Utilized to measure prediction accuracy, enabling us to assess model performance comprehensively.

| **Model**           | **Mean Squared Error (MSE)** | **Root Mean Squared Error (RMSE)** | **Root Mean Squared Logarithmic Error (RMSLE)** |
|----------------------|-------------------------------|------------------------------------|--------------------------------------------|
| **ARIMA**            | 0.0077                        | 0.0878                             | 0.0973                                     |
| **Linear Regression**| 0.0076                        | 0.0874                             | 0.0764                                     |
| **Decision Tree**    | 0.0147                        | 0.1211                             | 0.1061                                     |
| **XGBoost**          | 0.0023                        | 0.0477                             | 0.0415                                     |

3.  Model Hypertuning 
Applied grid search and cross-validation techniques to fine-tune hyperparameters, ensuring optimal XGBoost model configurations for accurate predictions. RMSLE = 0.03
## Outcomes
Our meticulously crafted models, honed through rigorous evaluation and optimization, yielded precise store sales forecasts. These forecasts provide Favorita with actionable insights, enabling informed decision-making and strategic planning
## Limitations 
It's essential to acknowledge the limitations of our analysis. Factors not included in the dataset, unforeseen events, or sudden market shifts might impact sales differently. Continuous monitoring and adaptation are key to addressing these limitations effectively.
## Conclusion
In conclusion, this Store Sales Forecasting project has showcased the power of time series analysis and advanced modeling techniques in predicting retail sales. By leveraging historical data and understanding the intricate relationships between various external factors and sales, Favorita is equipped with a robust forecasting tool. These insights not only enhance operational efficiency but also guide strategic initiatives, empowering Favorita to navigate the dynamic retail landscape with confidence. Continuous refinement and adaptation will be pivotal, ensuring Favorita remains agile and responsive to evolving market trends and customer preferences.
## Authors
| Name | GitHub link |
| ---- | ---- |
| Doe Edinam                   | https://github.com/doeabla         |
| Kofi Asare Bamfo             | https://github.com/akbamfo         |
| Enoch Taylor-Nketiah         | https://github.com/kojoboyoo       |
|Philip Tolutope Oludipe       |       |

| Project |	Name |	Published Article |	Deployed App |
| ---- | -----| ----- | ---- |
| LP3	| Regression_Analysis_SSP_LP3 |	[Time series LP3](https://medium.com/@eadoe97/predicting-favoritas-future-a-regression-analysis-approach-to-sales-prediction-79692378793f) | [Power BI Deployment](https://app.powerbi.com/groups/me/reports/9315022f-bf70-41c9-aedb-1ce535e07ec0/ReportSection?experience=power-bi) |
