#Analysis of SyriaTel performance in the Telecommunication Industry#

#Business Understanding

The telecommunication industry is faced with one of the fiercest competitions globally. Customers are in need of the cheapest, reliable and safe communication platforms.This study focuses on SyriaTel, a telecommunications company in Syria.Among the challenges facing this company include;Intense Competition,Service Quality Issues (Network Coverage and Reliability),Economic and Political Instability, Changing Customer Expectations,Pricing and Plan Flexibility,Customer Satisfaction and Perception,Regulatory Environment (Government Regulations),Inability to Predict Churn Patterns (Data Analysis Challenges and Lack of Insight into Customer Behavior. This study attempts to guide the mangement of SyriaTel on what areas to improve on in order to bring the company back to profitability.

#Business Problem

Syria Tel intends to turnaround their profitability. The management wants to esbablish roote causes of the challenges and how to address them. The business environment is competetive and the country is rocked with civil wars. The company is hopeful to navigate all these with a proper data analysis and recommendation. This study therefore focusses on customer behaviour with relation to the cost of call and messages, the duration of call and whether the costs should vary between days and nights.

#Data sources

SyriaTel Customer Churn Provides detailed data on various aspects of analysis including; account length, area code,phone number, international plan, voice mail plan,number of vmail messages, total day minutes, total day calls, total day charge, total eve calls, total eve charge, total night minutes, total night calls, total night charge and so on.

#Objectives

The objective of this study is to guide SyriaTel, based on analysis of the above data, how to respond to the changing market and political landscape in Syria.

#Data Understanding

#Data Processing

Modeling and Model Evaluation

#CONCLUSION

#Random Forest

Random Forest is the best performing model in terms of accuracy, precision, recall, and F1-score. Accuracy: 93.70% - High accuracy, suggesting the model is making correct predictions overall. Precision: 98.36% - Extremely high precision, indicating that when it predicts positives, it is very likely to be correct. However, its recall (59.41%) needs be improved

#Decision Tree

Is the second best with:Accuracy 91.60% - High accuracy and overall good performance. Precision: 71.03% - It predicts positives correctly with a good precision. Recall: 75.25% - It successfully identifies a large proportion of the positive cases Making it a good option if identifying positive cases is crucial.

#Logistic Regression

Logistic Regression has good accuracy but struggles with low recall and F1-score, so it may not be ideal if identifying positives is important. Accuracy: 85.76% - It has a decent accuracy but struggles with identifying positive cases, as reflected in its low recall (18.81%). Precision: 59.38% - It predicts positives correctly 59.38% of the time. Recall: 18.81% - It misses many positive instances.

#Support Vector Machine (SVM)

Is the worst Model here SVM is not usable as it fails to predict any positive cases, leading to zero precision, recall, and F1-score. Accuracy: 84.86% - Similar to Logistic Regression, but this is misleading as the model fails to identify any positives. Precision, Recall, and F1-Score: All are 0 because the model never predicts a positive class, making it useless in its current state. ROC AUC: 50.00% - It performs as well as random guessing.

#Recommendations

#Preferred Model: Random Forest

Based on the evaluation metrics, Random Forest stands out as the most effective model. It has the highest accuracy, excellent precision, recall, and F1-score. Its ROC AUC score of 0.80 confirms that it is good at distinguishing between churned and non-churned customers. This model should be the primary choice for predicting customer churn. It strikes a good balance between performance and interpretability. Additionally, Random Forest provides feature importance, which can offer valuable insights into the factors driving customer churn. Alternative Model: Logistic Regression

For a simpler, more interpretable model, Logistic Regression might still be useful. However, its low recall and F1-score indicate that improvements are needed. Consider fine-tuning hyperparameters or incorporating additional features that might help improve recall and overall performance. SVM:

SVM should be discarded for this particular task. The model’s failure to predict any churn cases and its poor ROC AUC score suggest that it is not suitable for this dataset. You could consider revisiting SVM after extensive tuning, but for now, Random Forest provides a much better solution.

#Next Steps

1.Focus on Model Improvement Random Forest and Decision Tree are the best performing models. However, Random Forest has a good balance of precision and recall, making it ideal for identifying potential churn. Since Decision Tree is also performing well, improving it through hyperparameter tuning or pruning can also enhance performance

2.Address Class Imbalance Many churn models suffer from class imbalance (where the number of churned customers is much smaller than non-churned customers). This could explain some of the low recall and performance issues, especially with Logistic Regression and SVM

3.Model Evaluation and Validation All models should be evaluated using cross-validation to ensure their performance is robust and not subject to overfitting. Since the data might be imbalanced, precision, recall, and F1-score should be prioritized, especially recall to ensure churned customers are being detected.
4.Customer Retention Strategies Use the churn prediction model to create actionable strategies for customer retention. For instance, if the model identifies high-risk customers, a targeted marketing campaign can be launched to offer promotions, improve customer service, or address specific customer pain points

5.Continuous Improvement & Feedback Loop Model Drift: Over time, customer behavior might change. Implement a feedback loop to continuously update and improve the model.

6.Business Collaboration and Insights Collaborate with the marketing, customer service, and product teams to ensure that churn insights are used effectively in business strategie

