
# Project #8: Car Price prediction Part2 (Neural networks, Computer Vision)
https://www.kaggle.com/polinafedosova/carpriceprediction2-polina-aleksandr-27b9a9
Public Score on Kaggle.com: 10.77901
## Goal:
to predict car price by its characteristics, text description or picture.
# Objectives:
- Let's build a "naive" / baseline model that predicts the price by model and year of manufacture (we will compare other models with it)
- tp process and normalize features
- to make the first model based on gradient boosting using CatBoost
- to make a second model based on neural networks and compare the results
- to build a multi-input neural network to analyze tabular data and text at the same time
- to add image processing to the multi-input network
- to build an ensemble of gradient boosting and neural network (averaging their predictions)
# Conclusion:
we carried out all the necessary work on data preparation, their analysis, processing and preparation for further work . The dataset is cleared of duplicates and outliers, normalization is performed, classical methods of coding categorical features were used. Additional features have been created. According to the results of the analysis, some of the features, including those based on correlation analysis, deleted. Classical language processing methods were used. We used tokenization and lemmatization in the model.
While working with images, we used our own augmentation code based on the albumentation library. Experiments have been carried out with other typical EfficientNet models,
some of which led to retraining. The Learning Rate adjustment was applied. Fine-tuning and Transfer Learning were also used.
As a result of blending, we managed to achieve good results of the metric 10.77901.

