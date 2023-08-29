# Customer Analytic Insight     
There are four categories of customer data analytics: **descriptive, diagnostic, predictive, and prescriptive**.     

- **Descriptive analytics**  helps you discover what happened in the past using historical data. It gives you insight into the causes of customer trends, as well as helps you prepare for the future.     

- **Diagnostic customer analytics** help you understand the “why” behind customer behavior by collecting user feedback and using hypothesis testing.     

- **Predictive analytics** helps you predict customers’ future performance and act on it.     

- **Prescriptive analytics** unlocks recommendations on what to do to fix an issue or the path you should take to achieve a goal.       

**Why customer analytics insights are important?**     

Gaining customer insights through analysis aids swift, informed business decisions. It helps your company as following example     

- Understand customer behavior and identify patterns
  
- Predict future customer behavior
  
- Segment your customers and personalize their experience
  
- Identify friction throughout the customer journey

  
[Reference user pilot website](https://userpilot.com/blog/customer-analytics-insights/)

# Example case of Customer Insight of Supermarket Tolus     
First step we have to understand business such as painpoint, strategy, and BU expectation.
- **Business objective** is to maximize profit in retail supermarket in Bangkok,Thailand  
- **Business Strategy** is to maintain Customer Retention  

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0e5c3d056e1b95c76d27b0fc8d2e8f5d5f04c7e3/2%20Customer%20Insight%20Analysis/Raw%20Data/Brand.png)
**Tolus's Expectaion**     

To turn member customer to loyalty customer expected to increase frequency and varaity of purchase product by 50% and increase customer spending by 30%  
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0e5c3d056e1b95c76d27b0fc8d2e8f5d5f04c7e3/2%20Customer%20Insight%20Analysis/Raw%20Data/Expectations.png)
# Data Preparation for Analytic by using RFM
Second, we have to understand data detail, data type, process and ownership in order to deal with it such as cleansing, data normalization or finding external source for fullfillment gap. In this case we use RFM as important feature.     


**RFM  
R: Recencies within 1 Months, 3 Months   
F: Frequency within 7 Months  
M: Monetary within 7 Months**  

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0e5c3d056e1b95c76d27b0fc8d2e8f5d5f04c7e3/2%20Customer%20Insight%20Analysis/Raw%20Data/RFM%20Data.png)
# Basic analysis
For understanding relationship of data by using correlation matrix, according to the graph mostly is prositive relation between variable such as recency 1 months VS total spend are positive correlation 69.5%.
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0e5c3d056e1b95c76d27b0fc8d2e8f5d5f04c7e3/2%20Customer%20Insight%20Analysis/Raw%20Data/Corrlation%20matrix.png)
# Clustering group of customer
The Clustering K Means at 5
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0e5c3d056e1b95c76d27b0fc8d2e8f5d5f04c7e3/2%20Customer%20Insight%20Analysis/Raw%20Data/Result.png)
Variable Important are recency 1 months VS total spend
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/5134cd0e81d65d9cf11a220849aa68783ff42ace/2%20Customer%20Insight%20Analysis/Raw%20Data/Viriable%20importance.png)
Scattle plot of recency 1 months VS total spend
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0e5c3d056e1b95c76d27b0fc8d2e8f5d5f04c7e3/2%20Customer%20Insight%20Analysis/Raw%20Data/ScatterPlot.png)
# Explaination variable relationship

The variaty in purchase item in each division from each Cluster (Total Division is 9)  
**- Cluster1** :  Mostly purchase product 4-6 divisions (Moderate)  
**- Cluster2** : Purchase product less than 3 divisions (The last)  
**- Cluster3** : Mostly purchase product 4-6 divisions  (Moderate)  
**- Cluster4** : Mostly purchase product 6-7 divisions (Good)  
**- Other** : Purchase product more than 6-8 divisions (The Best)  

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0e5c3d056e1b95c76d27b0fc8d2e8f5d5f04c7e3/2%20Customer%20Insight%20Analysis/Raw%20Data/ClusterbyFrequencyDivision.png)
The Recency of date that customer last purchase with us within 1 month (31/07/2008)  
**- Cluster 0** : Customer last purchase with us between 72 to 142 days (Nearly Churn)  
**- Cluster 1** : Customer last purchase with us between 25 to 88 days (Moderate)  
**- Cluster 2** : Customer last purchase with us between 25 to 81 days (Moderate)  
**- Cluster 3** : Customer last purchase with us between 136 to 212 days (Nearly Churn)  
**- Cluster 4** : Customer last purchase with us between 25 to 98 days (Moderate)  
**- Other** : Customer last purchase with us between 25 to 43 days (The Best)  

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0e5c3d056e1b95c76d27b0fc8d2e8f5d5f04c7e3/2%20Customer%20Insight%20Analysis/Raw%20Data/ClusterbyRecency1Month.png) 
Total Spend within 7 months (01/01/2008 to 31/07/2008)  
Cluster1 : Average total spending 50.55 (Mostly <150)___Moderate  
Cluster2 : Average total spending 1.17__Little Spend  
Cluster0 : Average total spending 25.96 (Mostly<50)___Little Spend  
Cluster3 : Average total spending 12.44 (Mostly<40)__Little Spend  
Cluster4 : Average total spending 561.93 (Mostly<600) ___Good  
Other : Average 1457.96 (Mostly<1,500) __TheBest  

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0e5c3d056e1b95c76d27b0fc8d2e8f5d5f04c7e3/2%20Customer%20Insight%20Analysis/Raw%20Data/ClusterbyTotalSpend.png)
