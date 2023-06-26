# Recommendations_with_IBM
 Udacity_Data_Science_NanoDegree_Project_Recommendation_Engine

## Project Overview
 **Sparkify** is a digital music service app, similar to Spotify or Pandora. Every day, numerous users engage with the Sparkify music streaming service by streaming their favorite songs. They have two options for accessing the service: the free tier, which includes intermittent advertisements played between songs, or the premium subscription model. With the premium subscription, users can stream music without interruptions and are charged a monthly flat rate. Users have the flexibility to upgrade, downgrade, or cancel their subscription at any time, based on their preferences and needs.

My goal is to predict which customer would cancel their subscription in the near future before they did so.
This is a typical `Customer Churn Prediction Problem`.

## Steps and Structure
- EDA (data exploration):
    - metric distribution
    - correlation between metrics
    - define churn
    - data clean
- Feature Engineering: select metrics with potential effects on the prediction churn. Prepare data for training.
- Model Training and Evaluation: for churn prediction, we use classification models. I chose Logistic Regression, Decision Tree, and Fandom Forest.
    - I trained the 3 models with baseline results and evaluated them;
    - Based on the evaluation results (I used F1 score as an evaluation measurement metric since the dataset was unbalanced), I chose the Logistic Regression model and the Decision Tree model for further tuning.
Model Tuning
    - I used the Grid-search method to do the tuning of the 2 selected models and received the best performances of both.
    - Since the Decision Tree Model has the best accuracy as well as the least training time, the final model selection step required no more evaluations.

## Installation

- Python 3.6
- Jupyter
- PySpark ML
- Pyspark SQL
- Matplotlib for visualization.
