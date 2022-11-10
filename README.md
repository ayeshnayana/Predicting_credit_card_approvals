# Predicting_credit_card_approvals

Predicting Credit Card Approvals¶
In this notebook, we will apply concepts of data wrangling to clean the data set and model. 
The last column in the data set contains the target, which will give us approvals and rejections. 
Missing data were handled by imputing the mode of each feature.

The cleaned data set was then modeled by using XGBoost and LightGBM. 
The sklearn RandomizedSearchCV was used to tune each model. 
We used 30 folds in the CrossValidation. The ROC_AUC score was obtained to quantify the accuracy of the model. 
Both XGB and LGB models have consistent AUC scores around 0.9-0.92. This score is a significant improvement compared to DiscisionTree Algorithms. 
Where DisicianTree algorithms consistently provided AUC scores around 0.8-0.85. 
The comparison between DisicisionTree, XGB, and LGB models was provided in a box plot. 
Finally, we used the ensemble voting method to obtain the ensemble model using DT, XGB, and LGB models. 
We used accuracy scores to quantify the model performance.
