# Churn Project     
- To explored and performed an analysis of an *e-commerce* dataset.     
- To ran different *classification algorithms* with sci-kit learn’s Pipeline method.     
- To used GreedsearchCV for hyperparameter tuning to find the best algorithm with the best set of parameters.     
Finally found out the features that had more influence on prediction.So, this was all about customer churn analysis and prediction.    
# Basic Churn Prediction     
[Basic Churn Prediction](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/11e6edc0f24e0c2aabe3b247ff95acbce688e084/4%20Churn%20Scoring/Raw%20Data/Python/Basic_Churn_Prediction.ipynb)     
[Ecommerce Churn Prediction](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/11e6edc0f24e0c2aabe3b247ff95acbce688e084/4%20Churn%20Scoring/Raw%20Data/Python/E_Commerce_Churn_Prediction.ipynb)
# E Commerce Churn Prediction     

**Goal**

- Predict the type of customer that has the potential to churn by identifying features to minimize customer churn rates and get the right business decisions.

**Objectives**

- Create a model to predict users who have the potential to churn and understand what features cause users to churn and features that spur potential to minimize churn rates.
- Optimizing the company’s revenue by grouping users who have the potential to churn so that they can be given different treatments so that the churn rate decreases.

**Exploratory Data Analysis**     
1. Categorical
   - Preferred Login  Device     
   - Preferred Payment Mode     
   - Preferred Order Cat     
   - Gender     
   - Marital Status     
3. Numerical
   - Customer ID
   - Churn
   - Tenure
   - City Tier
   - Warehouse To Home
   - Hour Spend On App     
   - Number of Device Registered
   - Satisfaction Score
   - Number of Address
   - Camplain
   - Order Amount Hike From Last Year
   - Coupon Used
   - Order Count
   - Day Since Last Order
   - Cashback Amount
   
From the dataset owned by shoptify, there are 20 feature datasets consisting of *5 categorical features* and *15 numerical features*.
     
**Feature Important**     
- The Tenure feature is very influential in identifying customer churn tendencies. The smaller the tenure, the more likely customers are to experience churn.      
- The Complain feature also affects the churn tendency of customers. The higher the complaint rate, the higher the tendency to churn.     

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/106419a858ac5e3e6a88f7dbdcfd4ae9346843c3/4%20Churn%20Scoring/Raw%20Data/FeatureImportant_EcommerceChurn.png)

**Confusion matrix**     
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/106419a858ac5e3e6a88f7dbdcfd4ae9346843c3/4%20Churn%20Scoring/Raw%20Data/Confusion%20matrix.png)

**Bivariate Analysis**     
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/106419a858ac5e3e6a88f7dbdcfd4ae9346843c3/4%20Churn%20Scoring/Raw%20Data/Bivariate%20Analysis.png)

**Multivariate Analysis**     

- The correlation between target churn features and tenure features is obtained with a correlation value of -0.34. The smaller the tenure value, the greater the churn rate.     
- Another feature correlation that is quite large is between the target churn feature and the complain feature with a correlation value of 0.25. The greater the complaint rate, the greater the churn rate.     

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/106419a858ac5e3e6a88f7dbdcfd4ae9346843c3/4%20Churn%20Scoring/Raw%20Data/Multivariate%20Analysis.png)

# Recommendation
To increase the service level in handling customer complaints by improving the products or services provided, such as automation of customer service and live chat.
