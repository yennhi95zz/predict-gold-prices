# Gold Price Forecasting
#### 🧑‍🏫 Author: [Nhi Yen](https://www.linkedin.com/in/yennhi95zz/)
##### 💡I write about Machine Learning on [Medium](https://medium.com/@yennhi95zz) || [Github](https://github.com/yennhi95zz) || [Kaggle](https://www.kaggle.com/nhiyen/code) || [Linkedin](https://www.linkedin.com/in/yennhi95zz/). If you found this article interesting, your support by giving me ⭐ will help me spread the knowledge to others.

## Introduction

This repository contains code for forecasting the price of gold using various time series forecasting methods. The dataset used is the daily price of gold in USD from 1950-01 to 2020-07.

## Dataset
The [Monthly Gold Price](https://www.kaggle.com/datasets/nhiyen/monthly-gold-price) dataset used for this analysis is the daily price of gold in USD from 1950-01 to 2020-07. The dataset contains 847 observations with 2 columns - Date and Price.

## Forecasting Models
The Jupyter notebook `Gold_Price_Forecasting_Models.ipynb` contains the code for building and evaluating three different time series forecasting models:

- Linear Regression Model
- Naive Model
- Exponential Smoothing Model

For the Linear Regression Model, the dataset was split into training and testing sets. The Linear Regression Model was fit on the training data and used to predict the gold prices for the test data. The mean absolute percentage error (MAPE) was used to evaluate the model's performance.

For the Naive Model, the last value of the training set was used to predict the gold prices for the test data. The MAPE was again used to evaluate the model's performance.

For the Exponential Smoothing Model, the statsmodels package was used to fit an Exponential Smoothing Model on the entire dataset. The model was then used to predict the gold prices for the test data. The 95% confidence intervals for the predictions were also calculated. The MAPE was again used to evaluate the model's performance.

## Results
The results of the three models were compared based on their MAPE scores. The Exponential Smoothing Model performed the best with a MAPE score of 17.235%.

![image](https://user-images.githubusercontent.com/88694623/229420633-73bd658e-34a1-4322-a5f8-58b800e8ad73.png)


## Conclusion
The Exponential Smoothing Model was used to predict the gold prices for the period 2020-08 to 2025-02. The predicted prices are stored in a CSV file named `gold_price_predictions.csv`.

## References
- Kaggle Dataset: [Monthly Gold Price](https://www.kaggle.com/datasets/nhiyen/monthly-gold-price)
- Github Repo - [HERE](https://github.com/yennhi95zz/predict-gold-prices)
- Kaggle Project - [HERE](https://www.kaggle.com/nhiyen/time-series-prediction-on-gold-prices)
- Time Series Visualization on [Tableau](https://public.tableau.com/views/TimeSeriesPredictiononGoldPrices/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link)
- Detail Explanation about the code on [MEDIUM]([https://medium.com/@yennhi95zz/unleashing-the-power-of-e-commerce-sales-analysis-a-case-study-4c64871a86ee](https://medium.com/@yennhi95zz/time-series-prediction-on-gold-prices-a826fc2ead0c))
