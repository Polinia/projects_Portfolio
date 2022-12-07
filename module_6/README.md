#	Project #6 'Recommendation Challenge'
https://www.kaggle.com/code/polinafedosova/recommendation-system-for-amazon
## Goals and objectives of the project: 
a development of a recommendation system for a large online retail company. The recommendation system should be based on the most accurate recommendation of the right product in a high price category.
## Data Description:

![2022-01-30 (3)](https://user-images.githubusercontent.com/68026029/151713090-92e4f472-8962-4a29-a60b-20f765992fe2.png)

Conclusion:
We have successfully completed a project for creating a recommendation system. We have prepared a series of sequential models to evaluate the project using the ROC AUC metric.
Which characterizes the accuracy of predictions and must be resistant to unbalanced classes.

We did a lot of work on EDA and Feature Engineering, however we decided to start with a simple model, that, as expected, did not give us the desired result, but good as a baseline.
The next step was to increase the data on which the model was trained - the result improved to 0.7495 on submission, which is already noticeably better than the baseline.
The next step was working with item_features and embeddings. Embeddings are lower dimensional vectors in machine learning. They are used to describe texts, images, videos, 
and more in search engines and recommendation engines. We need embeddings to give a prediction for each product, or rather, to look for the most similar ones. 
With the help of user/item_features we have added our features. If we use user/item_features in training, then LifhtFM considers that each user and item has one characteristic 
unique to that user (or item). For a quick search among a large number of products, we used the nearest neighbors method, approximate k-nn, which is implemented in the nmslib
library. Unfortunately, we did not use this model for the submission, since the metric we chose is close to 0.5.
