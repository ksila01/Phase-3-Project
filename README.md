# Phase 3 Project
important links:
** https://github.com/ksila01/Phase-3-Project/blob/main/Classification%20Modeling.ipynb
** https://github.com/ksila01/Phase-3-Project/blob/main/Data%20preparation.ipynb
** https://github.com/ksila01/Phase-3-Project/blob/main/Exploratory%20data%20analysis%20(EDA).ipynb
![project](https://github.com/ksila01/Phase-3-Project/blob/main/Images/download.jpg)
## Project Overview
Our client, SyriaTel is a telecommunication company with a severe loss of valuable customers to its rivals. Understanding and predicting customer churn is essential in assessing the effectiveness of the company's marketing efforts to improve customer satisfaction. In the telecom sector, user acquisition and retention are the main issues. Every business's marketplace is expanding quickly, which is leading to a rise in the number of subscribers. As a result, businesses now understand how important it is to keep their current clientele. Service providers now need to lower their client turnover rate because neglecting to do so could hurt their business's profitability. Churn prediction helps to determine which customers are most likely to move from one organization to another.
### Objectives
Objectives:

* Build a classifier model to determine whether a customer will soon churn from Syria Tell
* Establish the modeling with the best performance
* Determine features that influence customers' churn decisions
* Evaluate any predictable patterns
### Business Problem
Since the telecommunications business is growing to be one of the largest in the world, competition has intensified due to advancements in technology and the growing number of operators. Telecommunication companies are striving to survive in this competitive industry, and strategies have been developed to generate substantial profits. Companies must reduce the likelihood of customer churn, often known as "the movement of customers from one service provider to another service provider," in order to increase customer retention.  In service industries where there is a rise in competitive services, customer attrition is regarded as a serious problem.

### Data Understanding
The dataset provided information on the following features for each customer: 
![Churns vs state](https://github.com/ksila01/Phase-3-Project/blob/main/Images/newplot.png)
* US State
* Length of account
* Area code + phone numbers
* If the customer has an international plan
* If the customer has a voicemail plan
* No. of voicemail messages
* Breakdown of call minutes for day, evening, night, and international
* Breakdown of call charges for day, evening, night, and international
* Breakdown of no. of calls for day, evening, night, and international
* No. of calls to customer service
* If they have churned
#### DATA PREPARATION
The data contains 3333 unique values. No missing values, duplicates, or placeholders on the data
51 states are included in the dataset
#### EDA
California and New Jersey report the highest number of customers terminating their contracts with the company while those with the lowest churn are Alaska and Hawaii
![Churns vs customer service calls](https://github.com/ksila01/Phase-3-Project/blob/main/Images/churn%20customer%20service.PNG)

## Modeling
To achieve the objectives of this project, we utilized four classification models including;
** Logistic model
** K Nearest Neighbor 
** Decision Tree
** XG Boost Model
**** XG Boost outperformed all other models with an accuracy of 97.6%. The testing accuracy of 97.6% suggests that the XGBoost classifier performs exceptionally well on the testing dataset, with a high level of correct classifications.
Overall, the model exhibits excellent classification performance in both classes, with high precision and F1 scores, making it a strong candidate for this classification task.
![confusion matrix ](https://github.com/ksila01/Phase-3-Project/blob/main/Images/Confusion%20matrix.PNG)


We applied GridSearch to find the best parameters for our model and run our XGBoost classifier model with these parameters.

### Evaluation
To evaluate the performance of classification models, several evaluation metrics are commonly used. Here are some of the key evaluation metrics typically employed when assessing the performance of classification models:

Accuracy: Accuracy is a basic metric that measures the proportion of correctly classified instances in the dataset. It is calculated as the number of correct predictions divided by the total number of predictions.

Precision: Precision, also known as positive predictive value, measures the ability of the model to correctly identify positive instances among the instances it predicts as positive. It is calculated as the number of true positives divided by the sum of true positives and false positives. High precision indicates a low false-positive rate.

Recall (Sensitivity): Recall, also known as true positive rate or sensitivity, measures the ability of the model to correctly identify positive instances among all actual positive instances. It is calculated as the number of true positives divided by the sum of true positives and false negatives. High recall indicates a low false-negative rate.

F1-Score: The F1-score is the harmonic mean of precision and recall. It balances the trade-off between precision and recall and provides a single metric that considers both false positives and false negatives. It is calculated as 2 * (precision * recall) / (precision + recall).

ROC Curve and AUC: The Receiver Operating Characteristic (ROC) curve is a graphical representation of the model's ability to distinguish between positive and negative instances at different thresholds. The Area Under the ROC Curve (AUC) measures the overall discriminative power of the model. A higher AUC value indicates better discrimination.

Confusion Matrix: A confusion matrix provides a detailed breakdown of true positives, true negatives, false positives, and false negatives. It is a useful tool for understanding the performance of a classification model.

## Recommendations
It is evident from the feature analysis and the outcomes of the completed model that voice mail, international plans, and customer support calls have the most effects on customer attrition. SyriaTel has the following options for lowering churn:

Consumers who have contacted customer support more than three times ought to be given greater consideration. Monitor caller stats for customer support. Do customers phoning with the same concerns? We can better relieve these clients' pain by addressing and resolving these difficulties once we have an understanding of why they are calling.

Less than 10% of customers have the international plan and are paying the same price as those who do not have it, indicating an ineffective marketing campaign. The global strategy has to be revised.

## Conclusions
Our business's income is based on how satisfied our customers are. Establishing our priorities will help us concentrate. The most effective model for forecasting customer turnover behavior is the XGBoost Ensemble technique. According to both our model and the exploratory data study, some elements have a greater influence on the behavior of customers who churn. Customers tend to churn more quickly when they contact customer service more frequently, have an international plan, and do not have a voicemail plan. In order to avoid losing customers, we must address each issue separately.
