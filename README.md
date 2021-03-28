# Customer Churn Prediction Project


<p align="center">
  <img width="860" height="350" src="Images/readme.jpg">
</p>

## Business Problem
Syriatel telecommunication company hired a data scientist to build a classifier that can predict which customers will stop dealing with them for another provider, and identify how the company can avoid the loss of those customers.

### The Data

The Syriatel dataset is from the Kaggle website. The dataset consists of 3333 customers, 21 columns with different features (continuous and categorical). These features will help to understand which factor affects the customer's decision to stay or leave.

## Observasion

There is a significant target class imbalance because of approximately 86% of "False " and 14% of "True" This imbalance will affect our prediction,  I will deal with it by using SMOTE to balance the target.

![](images/Should%20I%20Stay%20or%20Should%20I%20Go.png)


Customers are more likely to leave if they call customer service more than three times

![](images/Customer_Services_calls.png)

42% of the customers who have an international plan will leave, so Syriatel should work on their international plan pricing

![](images/International_Plan.png)

### Conclusions
- There is a significant improvement in XGBoost Classifier after using SMOTE. The confusing matrix looks great with zero False Negative and False Positive.  The testing score is perfect on all metrics. There is a clear improvement from the previous XGBoost model.
- Customers who called customer service more than 3 times tend to leave.
- Customer who has international plan churn at a higher rate than the customer who has not.
- The top 5 churn's state are California, New Jersey, Texas, Maryland, and South Carolina,maybe they have bad coverage or competitive provider at those states; so customer service should pay special attention to those states



### Recommendations:
After looking at various feature importance from my final model, I would recommend the following measures to improve customer retention.
- Improve the quality of the customer service by offering more training.
- Customer service should follow-up with the customers who call 3 times and offer promotions or discounts like a free month.
- Syriatel should revisit its international plan and adjust the pricing.
- Syriatel should offer free voice mail plan for everyone.

### Limitaion
The size of the dataset and the limited features

### Future work
Looking for additional features like the coverage in some states and customer service rating.

