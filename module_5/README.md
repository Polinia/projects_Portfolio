# Project #5.	Car classification & price prediction
https://www.kaggle.com/polinafedosova/carpriceprediction-polina-aleksandr
## Objectives:
to create a model for car price prediction based on its characteristics.

## Data Description:

![2022-01-30 (2)](https://user-images.githubusercontent.com/68026029/151711602-a9b0cdeb-26c8-42c0-845f-b334104b1442.png)

# Conclusions
- CatBoost and GradientBoosting do a great job and show a good metric result, but xgboost showed the best result - 12.14%
- We recieve a better result after taking the logarithm of the target variable (CatBoost + log(target) = MAPE: 12.52%)
- We also managed to experiment with staking with various meta-algorithms (MAPE: 14.71%)
