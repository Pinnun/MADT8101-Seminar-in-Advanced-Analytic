# DATA ANALYTIC PROJECT      
## PROJECT OBJECTIVES    
There are analytic finding from data transactions as followings:    
1. One time visit in cluster "1" approx. 87%
2. Cluster 3, there are spread of no of visit in this cluster
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/b6f6c2a326c4f97762ccbf1e5b17e8d4a0dfcbbc/5%20Customer%20Segmentation_Product%20Recommendation/No%20of%20customer%20in%20each%20cluster.png)
Therefore, setting project objective to reach out to customers more effectively by increasingly personalized transactions and improve brand loyalty & customer lifetime value.

Therefore, the method using for reach the objective are Customer Segmentation and Product Recommendation. 
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/61105750795280daa4879a7afff0ecb195445541/5%20Customer%20Segmentation_Product%20Recommendation/1%20Obj1.jpg)
## DATA UNDERSTANDING     
Data analytice use case of HDI Corporate which have 2 files:     
1) Customer Data     
2) Sales Transaction 2021 - 2023     
- Sales transaction     
3 excel files from 2021 – 2023     
2,406,316 rows , 8 columns     
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/61105750795280daa4879a7afff0ecb195445541/5%20Customer%20Segmentation_Product%20Recommendation/1%20Data%20Understanding%201.png)
- Member data      
1 excel file     
590,565 rows , 5 columns     
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/61105750795280daa4879a7afff0ecb195445541/5%20Customer%20Segmentation_Product%20Recommendation/2%20Data%20Understanding%202.png)
## DATA PREPARATION        
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/61105750795280daa4879a7afff0ecb195445541/5%20Customer%20Segmentation_Product%20Recommendation/3%20SanityCheck1.png)
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/61105750795280daa4879a7afff0ecb195445541/5%20Customer%20Segmentation_Product%20Recommendation/4%20SanityCheck2.png)
## DATA TRANSFORMATION     
### Assumption
Assumption and limitation of data are:     
1. Focus on total amount by ignoring paid amount because there are only 50K members were paid more than zero from total customer around 578K members     
2. Using data from the most recent two months in 2023, recommend a product in each cluster.

![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/61105750795280daa4879a7afff0ecb195445541/5%20Customer%20Segmentation_Product%20Recommendation/5%20Data%20Transformation1.png)
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/61105750795280daa4879a7afff0ecb195445541/5%20Customer%20Segmentation_Product%20Recommendation/6%20Data%20Transformation2.png)
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
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/4fa3fc87b6cbdcad6af73e19fbd5a29e85eba6f7/5%20Customer%20Segmentation_Product%20Recommendation/7%20Feature%20Important.png)
#### Elbow
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/4fa3fc87b6cbdcad6af73e19fbd5a29e85eba6f7/5%20Customer%20Segmentation_Product%20Recommendation/8%20Elbow.png)
#### Silhouette
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/4fa3fc87b6cbdcad6af73e19fbd5a29e85eba6f7/5%20Customer%20Segmentation_Product%20Recommendation/9%20silhouette.jpg)
#### Scatter Plot
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/4fa3fc87b6cbdcad6af73e19fbd5a29e85eba6f7/5%20Customer%20Segmentation_Product%20Recommendation/10%20Scatter%20plot.jpg)
#### Cluster Explaination&Action
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/4fa3fc87b6cbdcad6af73e19fbd5a29e85eba6f7/5%20Customer%20Segmentation_Product%20Recommendation/11%20Customer%20Segmentation.png)
## PRODUCT RECOMMENDATIONS     
Using clustering data to recommend product within group.
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/d6fa6a969f2d34ccc689cd17dcf47ac2d569b91c/5%20Customer%20Segmentation_Product%20Recommendation/12%20Product%20Recommendation1.png)
Cosine Similarity
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/d6fa6a969f2d34ccc689cd17dcf47ac2d569b91c/5%20Customer%20Segmentation_Product%20Recommendation/13%20Product%20Recommendation2.png)
Matrix Member ID and Product with sum of quantity of product
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/d6fa6a969f2d34ccc689cd17dcf47ac2d569b91c/5%20Customer%20Segmentation_Product%20Recommendation/14%20Product%20Recommendation3.png)
Random select member ID to ranking user to user similarity
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/d6fa6a969f2d34ccc689cd17dcf47ac2d569b91c/5%20Customer%20Segmentation_Product%20Recommendation/15%20Product%20Recommendation4.png)
Example Product Recommendation in each cluster
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/d6fa6a969f2d34ccc689cd17dcf47ac2d569b91c/5%20Customer%20Segmentation_Product%20Recommendation/16%20Product%20Recommendation5.png)
Mock up Product Recommendation
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/d6fa6a969f2d34ccc689cd17dcf47ac2d569b91c/5%20Customer%20Segmentation_Product%20Recommendation/17%20Product%20Recommendation6.png)
## DASHBOARD     
Sales Dashboard
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0413136382060a4d9d7e93376530e140fe0f566a/5%20Customer%20Segmentation_Product%20Recommendation/Sales%20Dashboard.png)
Customer Dashboard
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/0413136382060a4d9d7e93376530e140fe0f566a/5%20Customer%20Segmentation_Product%20Recommendation/Customer.png)

## PERFORMANCE EVALUATION
![CDP Flow](https://github.com/Pinnun/MADT8101-Seminar-in-Advanced-Analytic/blob/d6fa6a969f2d34ccc689cd17dcf47ac2d569b91c/5%20Customer%20Segmentation_Product%20Recommendation/18%20Performance%20Evaluation.png)

