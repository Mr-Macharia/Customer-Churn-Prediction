
# Customer Churn Prediction

## Business Understanding

Syria Tel is a telecomunication company based in Damascus Syria. The company is experiencing an issue which they are losing customers after a given period of time. Therefore, to prevent further loss of customers to their competitors my goal is to understand the leads that result in the loss of customers. This is necessary since the insights derived from my analysis will be able to assist in the retaining of customers.

## Data Understanding.

There were 21 columns and 3333 rows.
14 were categorical and 7 numerical.


## Objectives

1. Analyse the problems causing the customer churns.
2. Create Models to implement the data.
3. Choose the best model.

## Project Summary

### EDA

The total is 2850 currently still customers and 483 that used to be customers. This accounts for about 15% of the total customers registered in the dataset.
The customers who remained did not rely mostly on the international plan.
Most unchurned customers did not utilize the voicemail plan.
The areacode 415 has the highest number of customers and churns.
The churn rate is higher than the retainment rate when the customer service calls are above 5.

### Modelling

The models used were;
1. Logistic Regression.
2. Decision Tree Classifier.
3. Random Forest Classifier.
4. XGBoost.

##### Model Performances:
1. **Logistic Regression** achieved 87% accuracy. It shows reasonably good precision (96%) for non-churn, but relatively lower recall (77%) and precision (52%) for churn.
  
2. **Decision Tree** achieved 84% accuracy. While it exhibited high precision (96%) for non-churn, the recall (76%) and precision (47%) for churn were comparatively lower.

3. **Random Forest** performed well with 92% accuracy. Showed balanced performance for both classes with high precision (95%) and recall (96%) for non-churn, and acceptable results for churn with 74% precision and 71% recall.

4. **XGBoost** emerged as the best model with 95% accuracy. The model demonstrated robust performance, especially in correctly classifying non-churn instances (96% precision, 98% recall), while maintaining reasonable precision (86%) and recall (77%) for churn.

#### Feature Importance:
- Across models, common influential features for churn prediction include `total day minutes`, `customer service calls`, `international plan`, `voicemail plan`, `and usage minutes` in various periods (evening, night).

The model that performed the best was the XGBoost with an accuracy of 95%.

### Recommendations
1. Reduce call charges for international plans, voicemail plans.
2. Improve call services by adding promotions.
3. Improve marketting and quality of services in area 510 and 408.
4. Improve marketing and service quality in Maryland, Texas and New Jersey.
5. Improve problem solving from insights gathered from customer service.
6. Create partnerships with other telecommunication companies along the area.
7. Create reward systems for customer charges to improve loyalty.