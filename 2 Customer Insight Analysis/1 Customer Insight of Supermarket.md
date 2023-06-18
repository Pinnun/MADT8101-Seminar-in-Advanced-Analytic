# Customer Insight of Supermarket Tulus
Business objective is to maximize profit in retail supermarket in Bangkok,Thailand  
Business Strategy is to maintain Customer Retention  

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/1fe4615448610cd819ba7e3a1b46236904c9fd8b/2%20Customer%20Insight%20Analysis/Brand.png)
# Tulus's Expectaion
To turn member customer to loyalty customer expected to increase frequency and varaity of purchase product by 50% and increase customer spending by 30%  
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/a7e1ad28a965bdf82003f3b55902efedad6799ce/2%20Customer%20Insight%20Analysis/Expectations.png)
# Data Preparation for Analytic by using RFM
RFM  
R: Recencies within 1 Months, 3 Months   
F: Frequency within 7 Months  
M: Monetary within 7 Months  

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/853d85812c6adb1a096dff1ceb067f2a9aa488a9/2%20Customer%20Insight%20Analysis/RFM%20Data.png)
# Analysis by using correlation matrix
According to the graph mostly is prositive relation between variable such as recency 1 months VS total spend are positive correlation 69.5%.
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/d47e06da241aa8751d6ad49a30eaafcb3c414442/2%20Customer%20Insight%20Analysis/Corrlation%20matrix.png)
# Clustering group of customer
The Clustering K Means at 5
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/1c387a16e188e5c7c320e5a6fd9d29f2f6de2db0/2%20Customer%20Insight%20Analysis/Result.png)
Variable Important are recency 1 months VS total spend
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/39a2cf5ec6ad66c991e90db042b812ff7f563782/2%20Customer%20Insight%20Analysis/Viriable%20importance.png)
Scattle plot of recency 1 months VS total spend
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/b2a276756a977a073c74750b570cac48648b1054/2%20Customer%20Insight%20Analysis/ScatterPlot.png)
# Expanation variable relationship
The variaty in purchase item in each division from each Cluster (Total Division is 9)  
Cluster1 :  Mostly purchase product 4-6 divisions (Moderate)  
Cluster2 : Purchase product less than 3 divisions (The last)  
Cluster3 : Mostly purchase product 4-6 divisions  (Moderate)  
Cluster4 : Mostly purchase product 6-7 divisions (Good)  
Other : Purchase product more than 6-8 divisions (The Best)  

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/5df312be4ad9a9306641d7c63014709431bd9501/2%20Customer%20Insight%20Analysis/ClusterbyFrequencyDivision.png)  
The Recency of date that customer last purchase with us within 1 month (31/07/2008)  
Cluster 0 : Customer last purchase with us between 72 to 142 days (Nearly Churn)  
Cluster 1 : Customer last purchase with us between 25 to 88 days (Moderate)  
Cluster 2 : Customer last purchase with us between 25 to 81 days (Moderate)  
Cluster 3 : Customer last purchase with us between 136 to 212 days (Nearly Churn)  
Cluster 4 : Customer last purchase with us between 25 to 98 days (Moderate)  
Other : Customer last purchase with us between 25 to 43 days (The Best)  

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/5df312be4ad9a9306641d7c63014709431bd9501/2%20Customer%20Insight%20Analysis/ClusterbyRecency1Month.png)
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/5df312be4ad9a9306641d7c63014709431bd9501/2%20Customer%20Insight%20Analysis/ClusterbyTotalSpend.png)
