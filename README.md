# Customer Segmentation using E-commerce Data
This repository contains a comprehensive customer segmentation project that leverages an online retail dataset to identify distinct customer groups. The project is divided into two main parts, each in its own Jupyter Notebook, guiding you from raw data exploration to actionable business insights.

The primary goal is to transform transactional data into meaningful customer profiles using feature engineering and unsupervised clustering algorithms. By understanding different customer archetypes, a business can tailor marketing strategies, improve customer retention, and personalize user experience.

## Structure at a Glance
This repository is organized into two main projects, each contained within its own Jupyter Notebook, representing a complete pipeline from data preparation to modeling and interpretation.

### 1. EDA and Feature Engineering for Customer Segmentation

[View EDA & Feature Engineering Notebook](http:https://github.com/MinaGong/customer_segmentation/customer_segmentation_feature_engineering.ipynb)

This project focuses on the foundational data preparation required for effective clustering. The goal is to deeply understand the raw transaction data and engineer a rich set of features that capture customer purchasing habits, preferences, and engagement levels.

**Key Steps**:

* **Exploratory Data Analysis (EDA)**: Performed an in-depth analysis of the dataset, including data cleaning, outlier detection, and examination of feature distributions.

* **Time Series Analysis**: Investigated transaction patterns over time to identify yearly, weekly, and daily seasonality.

* **Text Analysis & Product Categorization**: Processed product descriptions to extract keywords and create high-level product categories (e.g., Home Decor, Kitchenware, Gift & Seasonal).

* **RFM Feature Engineering**: Created classic Recency, Frequency, and Monetary (RFM) metrics to quantify customer value and loyalty.

* **Data Preprocessing**: Standardized numerical features and one-hot encoded categorical variables to prepare the dataset for machine learning models.

### 2. Customer Segmentation with Clustering Algorithms

[View Clustering Notebook](http:https://github.com/MinaGong/customer_segmentation/customer_segmentation_clustering.ipynb)

This project takes the engineered features and applies unsupervised learning to group customers into meaningful segments. The goal is to build, evaluate, and interpret clusters that represent different types of customer behavior, such as high-value loyalists, occasional shoppers, and lapsed customers.

**Key Steps** :

* **K-Means Clustering**:

    * Used the Elbow Method to determine the optimal number of clusters.
    * Trained the model and analyzed the resulting segments, identifying key profiles like "High-Value & Frequent Shoppers" and "Lapsed Customers."

* **DBSCAN Clustering**:

    * Utilized a k-distance plot to find the optimal eps parameter.
    * Applied this density-based approach as an alternative method for identifying core customer groups and outliers.

* **Model Evaluation & Comparison** :

    * Calculated the Silhouette Score to quantitatively measure the quality and separation of the clusters from both models.

* **Visualization and Interpretation** :

    * Used Principal Component Analysis (PCA) to visualize the customer segments in 3D space.

Derived actionable business insights from the characteristics of each identified customer cluster to inform marketing and strategy.

* **K-Means Cluster Profiles** : Understanding Your Customers
The K-Means algorithm successfully identified three distinct customer segments, which are clearly separated when visualized with PCA. 

1. **Cluster 0**
    Seasonal Weekend Buyers (15%): Moderate spenders, weekend + holiday-driven.
2. **Cluster 1**  
    Niche Frequent Weekday Buyers (6%): Small group, very frequent on weekdays.
3. **Cluster 2** 
    Christmas-Driven Weekday Buyers (37%): Largest cluster, moderate spenders, strong holiday focus.
4. **Cluster 3** 
    VIP Loyalists (27%): High-frequency, high-spending, weekday daytime customers, consistent year-round.
5. **Cluster 4** 
    Night-Active Steady Buyers (15%): Balanced spenders with unusual night-time activity.
