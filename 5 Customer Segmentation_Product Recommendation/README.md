# DATA ANALYTIC PROJECT      
## PROJECT OBJECTIVES    
There are analytic finding from data transactions as followings:    
1. One time visit in cluster "1" approx. 87%
2. Cluster 3, there are spread of no of visit in this cluster
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/No%20of%20customer%20in%20each%20cluster.png)

Therefore, setting project objective to reach out to customers more effectively by increasingly personalized transactions and improve brand loyalty & customer lifetime value.

Therefore, the method using for reach the objective are Customer Segmentation and Product Recommendation. 
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/12%20Product%20Recommendation1.png)
## DATA UNDERSTANDING     
Data analytice use case of HDI Corporate which have 2 files:     
1) Customer Data     
2) Sales Transaction 2021 - 2023     
- Sales transaction     
3 excel files from 2021 – 2023     
2,406,316 rows , 8 columns     
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/1%20Data%20Understanding%201.png)
- Member data      
1 excel file     
590,565 rows , 5 columns     
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/2%20Data%20Understanding%202.png)
## DATA PREPARATION        
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/3%20SanityCheck1.png)
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/4%20SanityCheck2.png)
## DATA TRANSFORMATION     
### Assumption
Assumption and limitation of data are:     
1. Focus on total amount by ignoring paid amount because there are only 50K members were paid more than zero from total customer around 578K members     
2. Using data from the most recent two months in 2023, recommend a product in each cluster.

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/5%20Data%20Transformation1.png)
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/6%20Data%20Transformation2.png)
## CUSTOMER SEGMENTATION     
### ML Result     
Customer Record : 325,164 rows     
Silhouette : 0.553      
KMeans : 3 Clusters   
Features Use :
- Order size,     
- Number of visit,      
- Mean time between purchase,      
- CLTV,      
- Visit period,      
- Total amount,      
- Basket size,    
- Total quality,     
- Visit size,      
- No of center,      
- Transaction price Q4,      
- Discount amount,      
- No of downline
#### Feature Important     
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/7%20Feature%20Important.png)
#### Elbow
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/8%20Elbow.png)
#### Silhouette
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/9%20silhouette.jpg)
#### Scatter Plot
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/10%20Scatter%20plot.jpg)
#### Cluster Explaination&Action
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/11%20Customer%20Segmentation.png)
## PRODUCT RECOMMENDATIONS     
Using clustering data to recommend product within group.
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/12%20Product%20Recommendation1.png)
Cosine Similarity
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/13%20Product%20Recommendation2.png)
Matrix Member ID and Product with sum of quantity of product
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/14%20Product%20Recommendation3.png)
Random select member ID to ranking user to user similarity
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/15%20Product%20Recommendation4.png)
Example Product Recommendation in each cluster
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/16%20Product%20Recommendation5.png)
Mock up Product Recommendation
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/17%20Product%20Recommendation6.png)

## DASHBOARD     
Sales Dashboard
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/Sales%20Dashboard.png
)
Customer Dashboard
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/Customer.png)

## PERFORMANCE EVALUATION
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/445107beea8634d3a3f20d0cb3d6feebd320d5e4/5%20Customer%20Segmentation_Product%20Recommendation/Raw%20Data/18%20Performance%20Evaluation.png)

