# Customer Segmentation Analysis

## Project Overview

This project focuses on segmenting an e-commerce company's customers based on their purchasing behavior.

The main goal is to identify different customer groups using **RFM analysis** and **K-Means clustering**. These segments can help the company understand customer behavior and create more targeted marketing strategies.

## Objectives

* Explore and understand the customer dataset
* Clean and prepare the data
* Perform RFM (Recency, Frequency, Monetary) analysis
* Select important customer behavior features
* Standardize the data using `StandardScaler`
* Determine the optimal number of clusters using the Elbow Method
* Apply the K-Means clustering algorithm
* Visualize customer segments
* Analyze and describe each customer group
* Provide marketing recommendations for each segment

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## Dataset

The dataset contains customer purchase information, including:

* Customer ID
* Purchase Date
* Product Category
* Product Price
* Quantity
* Total Purchase Amount
* Payment Method
* Customer Age
* Returns
* Customer Name
* Age
* Gender
* Churn

For the clustering analysis, the main features used were:

* **Recency** — how recently a customer made a purchase
* **Frequency** — how often a customer made a purchase
* **Monetary** — how much money a customer spent

## Project Workflow

### 1. Dataset Loading and Initial Exploration

The dataset was loaded using Pandas and its structure, columns, data types, and missing values were checked.

### 2. Data Cleaning and Preprocessing

Missing values and duplicate records were checked. The data was prepared for further analysis.

### 3. RFM Analysis

Customer-level RFM features were calculated:

* Recency
* Frequency
* Monetary

### 4. Descriptive Statistics

Basic statistical information was calculated to understand customer purchasing behavior.

### 5. Feature Selection and Standardization

The three RFM features were selected for clustering and standardized using `StandardScaler`.

### 6. Elbow Method

The Elbow Method was used to find a suitable number of clusters for the K-Means algorithm.

### 7. K-Means Clustering

K-Means was applied to group customers with similar purchasing behavior.

### 8. Cluster Visualization

The clusters were visualized using scatter plots, including:

* Recency vs Monetary
* Frequency vs Monetary

### 9. Cluster Profiling

The average Recency, Frequency, and Monetary values were calculated for each cluster.

The final customer groups were:

| Cluster | Customer Type                | Customers |
| ------- | ---------------------------- | --------: |
| 0       | Inactive Customers           |     7,588 |
| 1       | Loyal / High-Value Customers |     8,236 |
| 2       | Low-Activity Customers       |    15,199 |
| 3       | Active / Potential Customers |    18,638 |

## Key Insights

### Cluster 0 — Inactive Customers

Customers in this group have a very high Recency value and relatively low purchase frequency and spending.

**Recommendation:** Use re-engagement campaigns, special discounts, and personalized offers.

### Cluster 1 — Loyal / High-Value Customers

This group has the lowest Recency and the highest Frequency and Monetary values. They are the most valuable customers.

**Recommendation:** Use loyalty programs, VIP offers, exclusive discounts, and retention strategies.

### Cluster 2 — Low-Activity Customers

These customers have relatively low purchase frequency and spending.

**Recommendation:** Use targeted promotions, product recommendations, and discounts to increase their activity.

### Cluster 3 — Active / Potential Customers

This is the largest customer group. These customers are relatively active and have good potential to become high-value customers.

**Recommendation:** Use personalized recommendations, cross-selling, upselling, and loyalty campaigns.

## Conclusion

Customer segmentation helps businesses understand that different customers have different purchasing behaviors.

The K-Means clustering approach identified four customer segments with different levels of activity, purchase frequency, and spending. These results can help the company create more personalized marketing strategies and improve customer retention and engagement.

## Project Structure


Customer-Segmentation-Analysis/
│
├── customer_segmentation.ipynb
├── dataset/
│   └── customer_data.csv
├── README.md
└── images/
    ├── elbow_method.png
    ├── recency_monetary.png
    ├── frequency_monetary.png
    └── cluster_distribution.png

## Author

**Hajar Ibrahimli**

Data Analytics / Data Science Student
