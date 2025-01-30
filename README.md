# RFM-Analysis-for-Customer-Segmentation
RFM Analysis for Customer Segmentation applies the Recency, Frequency, and Monetary (RFM) model with K-Means clustering to classify customers based on purchasing behavior. This helps businesses optimize marketing, improve retention, and maximize revenue through targeted engagement strategies.

This project focuses on customer segmentation using the RFM model (Recency, Frequency, Monetary Value) to drive targeted marketing strategies. By segmenting customers based on their purchasing behavior, this analysis has the potential to generate millions of dollars in revenue for the organization.

## RFM Model Explanation

- **Recency (R):** How recently a customer made a purchase.
- **Frequency (F):** How often a customer makes a purchase.
- **Monetary Value (M):** How much money a customer spends on purchases.

Based on these three factors, a K-Means clustering model is used to classify customers into distinct segments.

## Dataset Used

The dataset includes the following attributes:

- **Invoice No:** Unique invoice number for each transaction.
- **Quantity:** Number of items purchased.
- **Invoice Date:** Date of purchase.
- **Unit Price:** Price per unit of the product.
- **Customer ID:** Unique identifier for each customer.
- **Country:** Country of the customer.

## Data Preprocessing

1. **Calculating Recency**
   - Recency is determined by measuring the time since the customer’s last purchase.
   - Since this dataset is not real-time, 2021-01-01 was set as the present date, considering the most recent purchase date in the dataset is 2010-12-09.

2. **Calculating Frequency & Monetary Value**
   - **Frequency:** The total number of purchases made by each customer.
   - **Monetary Value:** The total spending of each customer.

3. **Standardizing the Dataset**
   - Standardization ensures that all features are on a common scale, improving the performance of the machine learning model.

## Model Implementation

- K-Means Clustering was used for segmentation.
- The Elbow Method was applied to determine the optimal number of clusters, which was found to be 3.
- The model was trained with three clusters, and customers were classified accordingly.

## Cluster Analysis

The mean values of Recency, Frequency, and Monetary Value for each cluster are as follows:

| Cluster | Recency | Frequency | Monetary Value |
|---------|---------|-----------|----------------|
| 1       | 62      | 6         | 1,795          |
| 2       | 268     | 2         | 460            |
| 3       | 28      | 84        | 75,967         |

Based on the RFM values, the following customer classifications were derived:

| Customer Type | Cluster | Definition |
|---------------|---------|------------|
| **Whale Customers** | 3 | Low recency, high frequency, and high monetary value. |
| **Average Customers** | 1 | Higher recency than whales, lower frequency and monetary value. |
| **Lapsed Customers** | 2 | Highest recency with low frequency and monetary value. |

### Customer Distribution

- **Whale Customers:** 26
- **Average Customers:** 3,239
- **Lapsed Customers:** 1,107

## Recommendations

### 1. Targeting Average Customers

- The marketing team should focus on the 3,239 average customers by offering promotions, loyalty programs, or discounts to encourage more frequent purchases.
- Converting even a fraction of these customers into high-value customers could significantly increase revenue.

### 2. Re-Engaging Lapsed Customers

- While reactivating lapsed customers is challenging, implementing strategies such as personalized offers, email campaigns, and exclusive deals could help regain at least 10 percent of them.
- Even a 10 percent reactivation rate would provide substantial business value.

By implementing these targeted strategies, the organization can maximize revenue growth and enhance customer engagement.


