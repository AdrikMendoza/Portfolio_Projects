# Tasty Bytes (E-Commerce Website) - Binary Classification Model

## Company Background

Tasty Bytes , an online recipe startup, has hired you as a data scientist. The website features new recipes on the homepage every day. The owner has told you that on days that they feature a popular recipe, traffic increases by as much as 40%. However, it is difficult to predict in advance which recipes will be popular.

Recipes are considered to be popular if they receive a high score. The data team has collected data from previously published recipes.


Link of the Presentation: [(Click Here)](https://www.canva.com/design/DAFL7-NdRdI/CwuHyPK2N7AfAu9buMNkDA/view?utm_content=DAFL7-NdRdI&utm_campaign=designshare&utm_medium=link&utm_source=homepage_design_menu)


### Customer Question

The owner wants to know:
- Can you use information on previously published recipes to predict whether a recipe will receive a high score?



### Success Criteria

**The owner estimates that of all low scoring recipes, they currently correctly categorize 75% of them.** They want to know how your approach compares to this.

In order to predict whether or not a recipe will receive a low score, we need to preprocess the data. However, let's figure out what is the challenge about. The data have labeled data where 1 is a high score, and 0 is a low score. Than means, we are going to predict if a recipe will be unpopular. Hence, it is a binary classification challenge.

**OBJECTIVE: Create a binary classification model to predict low scoring recipes. This means, that the model should have a good rate of Negative Predictive Value.**


### About the Dataset

* **`RecipeId`:** Unique identifier of recipe.
* **`Name`:** Name of recipe.
* **`RecipeCategory`:** Type of recipe. (Dessert, Breakfast, etc)
* **`Calories`:** Number of calories.
* **`CholesterolContent`:** Amount of cholesterol in milligrams.
* **`CarbohydrateContent`:** Amount of carbohydrates in grams.
* **`SugarContent`:** Amount of sugar in grams.
* **`ProteinContent`:** Amount of protein in grams.
* **`RecipeServings`:** Number of servings.
* **`HighScore`:** Where 1 is a high score and 0 is a low score.


## Conclusions

In conclusion, the data was cleaned handling missing values, and outliers. Furthermore, the data was preproccesed oversampling observations because of an imbalance in data, and finally scaling features. In summary, found that the best performing model was a Random Forest Classification approach which has achieved:

1. A 75.57% accuracy with hyperparameter tuning.
2. Finding that the most important features are: `Calories`, `CarbohydrateContent`, `ProteinContent`, `SugarContent`, `CholesterolContent`, in that order.
3. Evaluating the ROC Curve with a Sensitivity score of 78.05% and Specificity score of 73.14%.
4. A ROC AUC Score of 0.8196 which means that the model is 62% better than a model randomly guessing. 
5. A Negative Predictive value of 77.32% and a Positive Predictive Value of 73.97%.
6. The model have reached a 73.14% of correctly classifying Low Scoring recipes which is 1.86% less than 75%. However, comparing the NPV of 77.32% to the success criteria, we improved the probability of classifying correctly a low scoring recipe in 2.32%.


## Recommendations

1. Getting more relevant features in relation to traffic of every recipe like: impressions, clicks, number of purchases, etc.
2. Proposing that focusing focusing on predicting high scoring recipes. It is more essential to correctly classify a High Scoring recipe because in that way we would get more chances to get 40% more traffic for future recipes.
