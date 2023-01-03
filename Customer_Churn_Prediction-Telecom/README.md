# Customer Churn Prediction Model for a Telecom Company

**Customer churn, also known as customer turnover, refers to the percentage of customers who stop doing business with a company over a certain period of time.**

A binary prediction model for customer churn is a statistical model that is used to predict whether a customer is likely to churn or not. This type of model is often used by businesses to identify customers who are at risk of leaving and take proactive measures to try to retain them. The goal of the model is to predict churn with a high level of accuracy, so that the business can focus its efforts on the customers who are most likely to churn.

# Conclusions
In conclusion, the data was cleaned handling duplicated values. Furthermore, the data was preproccesed using encoding for categorical variables, and finally scaling features. In summary, found that the best performing model was a Losgistic Regression for Classification approach which has achieved:

1. A 80.66% accuracy with hyperparameter tuning.
2. The largest effects on the odds of churning are: `tenure`, `Contract_Two year`.
3. Evaluating the ROC Curve with a Sensitivity score of 54% and Specificity score of 91.97%.
4. A ROC AUC Score of 0.8587 which means that the model is more than 60% better than a model randomly guessing. 

# Recommendations

1. Defining the business case for further tuning of the model, giving priority for negative predictive values or positive predictive values.
2. The model performs very well predicting not churners, we can use this on a specific business case context. For example: Keep customers and Acquiring more customer.
