# RFM Analysis for Customer Segmentation

![](Customers_segmented.png)

### Why Customer Segmentation?
Understanding customer behavior is crucial for targeted marketing. 

RFM Analysis helps businesses identify high-value customers and optimize marketing strategies.

RFM Analysis helps businesses identify their best customers and create personalized marketing campaigns.

This project uses real-world customer data to apply RFM segmentation.

## Overview
This repository contains the **RFM (Recency, Frequency, Monetary) Analysis** notebook used for customer segmentation. The analysis aims to segment customers based on their purchasing behavior, which helps businesses identify high-value customers and tailor marketing strategies accordingly.


## Project Structure
📌 **Data**: The folder where datasets used for analysis are stored (e.g., CSV files).

📌 [**Data Processing in Databricks**](RFM_Preprocessing.ipynb): several preprocessing steps were performed to clean and prepare the data for analysis.

✅ Loaded & Explored Data (CSV files into Databricks)

✅ Checked for Missing Values & Duplicates (Handled null values & removed duplicate transactions)

✅ Transformed Data Types 

✅ Performed Data Filtering 

✅ Applied Joins & Aggregations (Merged datasets based on customer ID)

📌 [**RFM Analysis & Modeling in Jupyter Notebook**](RFM_Analysis.ipynb):

✅ Loaded Preprocessed Data from Databricks into Jupyter Notebook

✅ Performed RFM Computations
  
1. **Recency** (R): Days since last purchase
   
   How recently did the customer make a purchase?  

   This metric identifies the freshness of the customer’s last purchase.
   
2. **Frequency** (F): Number of transactions
   
   How often does the customer make a purchase?

   This indicates how loyal the customer is to the brand.
   
3. **Monetary** (M): Total purchase amount
   
   How much money did the customer spend?

   This shows the value of the customer based on their spending.

✅ Implemented Multiple RFM Segmentation Techniques:

* Simple Quartile-Based Segmentation (Divided RFM values into quartiles)
* Separate R, F, M Analysis (Analyzed each RFM metric separately)
* Rank & Normalization Approach (Used z-score and Min-Max scaling for better comparability)

✅ RFM Score Segmentation (Summed up RFM ranks to assign customer segments)

✅ Different Quartile EDA for Top Customers (Explored quartiles differently to spot key customers)

✅ Applied Data Transformations:

* Log Transformation to handle skewness in Frequency & Monetary values
* Normalization to ensure better clustering results
  
✅ Clustered Customers for Advanced Segmentation:

* K-Means Clustering for unsupervised segmentation
* Elbow Method & Silhouette Score to determine optimal clusters
  
✅ Generated Final Customer Segments & Insights:

* Identified Best (High-Value), At-Risk, and Dormant Customers

✅ Prepared data for Power BI Dashboard visualization


## Key Insights
- Identify **high-value customers** for targeted marketing.
- Segment customers into **different groups** based on their RFM scores.
- Optimize **marketing campaigns** to retain loyal customers and improve acquisition strategies for less engaged customers.



