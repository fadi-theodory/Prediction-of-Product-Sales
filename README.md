# Tuned random forest for Prediction-of-Product-Sales
**Author**: Fadi Theodory
### Business problem:
The first project will be a sales prediction for food items sold at various stores. The goal of this is to help the retailer understand the properties of products and outlets that play crucial roles in increasing sales.
# Methods
We would dive into data to understand what does affect the sales
Sales prediction for food items sold at various stores
#### Visual 1: Outlet size vs sales
![Outlet size vs sales](https://github.com/user-attachments/assets/f536f3df-37db-4717-a613-540fda76db0f)
#### Visual 2: Outlet Size vs Item Outlet Sales divided by location type

![Outlet Size vs Item Outlet Sales divided by location type](https://github.com/user-attachments/assets/36fd3a37-dc3a-462a-a74e-1c822802538c)



## Results
> in Visual 1, we could see that the medium outlet size has the highest sales.
> in Visual 2, we noticed that tier 3 in the medium size is the highest sales.


## Model

We used linear regression and random forest regressor
the metrics for random forest were as followig:
**Results of the tuned random forests Regression Metrics: Training Data**

MAE = 653.581

MSE = 868,838.966

RMSE = 932.115

R^2 = 0.706

**Regression Metrics: Test Data**

MAE = 734.559

MSE = 1,118,876.716

RMSE = 1,057.770

R^2 = 0.594

we can see that the model is over fitting

However, i

Refer to the metrics to describe how well the model would solve the business problem

## Recommendations:

We will use the tunned random forest, because it is less overfitting than the untuned and the linear regression model

Yet, maybe the parameters should be changed to get better results. However, it took 15 minutes for this model to perform, I don't think it is practical to change the parameters again

Our model can explain about 60% of the testing data, and 70% from the training data it explains better on the training data, but still makes mistakes on the testing data.

MAE Mean aboslute Error

for training data MAE is 653.581, and  734.559 for test data.

this means that if we add all the errors (differnce between prediction and actual) in the testing data and took the average for them, the resul is 653 same for the test data, but with an average of 734. that means that the model is performing better on the training data then the testing data

Why you selected this metric to explain to your stakeholder?

Mean absolute error is the easiest metric to comprehend. Explaining it makes sense. it is the mean of the sum of all errors. on average, the training data prediction is different than the actual value by 653 point
-   

##We determined the best coefficient for both linear regression function and random forest

### Linear Regression
![Linearregression coeff](https://github.com/user-attachments/assets/ab9d0c83-d97d-4fbb-8140-c0f54590f59a)

the top impactful features are 


1.  Outlet Identifier- out27. product sold in the outlet 27 increases  the sales increase by `585`. 

2.   OUTLET TYPE supermarket type 3 same as before
3.   Outlet type grocery store. for items sold in outlet type grocery store, the saes will decrease by `884.691`


### Random forest
![Random forrest coeff](https://github.com/user-attachments/assets/a45b83ee-fc0c-4a6a-bc68-94ff9819c522)

The most important 5 features are:



1.   Item MRP 
2.   Outlet type grocery store
3.   Item Visibility
4.   Item weight
5.   outlet Type supermarket 3

## For further information
Should you need more clarifications,  please contact us at 

 
