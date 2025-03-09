# Unsupervised-Learning-Clustering-

## Project Overview
This project involves performing customer segmentation on credit card users using clustering techniques. The dataset includes customer transaction data over a six-month period. The goal is to identify distinct customer groups to optimize marketing strategies.

## Dataset Description
- **CUST_ID**: Unique identifier for each customer (Categorical)
- **BALANCE_FREQUENCY**: Frequency of balance updates (0 to 1)
- **PURCHASES**: Total purchase amount
- **CASH_ADVANCE**: Cash advances taken by the user
- **CREDIT_LIMIT**: Maximum credit allowed for the user
- **PAYMENTS**: Total payments made by the user

## Steps Performed
### 1. Data Import and Exploration
- Loaded the dataset and performed basic exploration.
- Checked for missing values and data inconsistencies.

### 2. Data Preparation
- Handled missing values in **CREDIT_LIMIT** using the median.
- Removed outliers from **PURCHASES**, **PAYMENTS**, and **CASH_ADVANCE** using the IQR method.

### 3. Hierarchical Clustering
- Used hierarchical clustering with **PURCHASES** and **CREDIT_LIMIT**.
- Generated a dendrogram to determine the optimal number of clusters.
- Assigned cluster labels and visualized the results.

### 4. K-Means Clustering
- Applied K-Means clustering for customer segmentation.
- Used the **Elbow Method** to determine the optimal number of clusters.
- Visualized the clusters based on **PURCHASES** and **CREDIT_LIMIT**.

### 5. Saving the Model and Results
- Saved the trained K-Means model using `joblib`.
- Saved the clustered dataset as a CSV file for future reference.

## Results and Interpretation
Three customer segments were identified:
1. **Low Spenders, Low Credit Limit**: Inactive or low-usage customers.
2. **Moderate Spenders, Mid Credit Limit**: Regular users with moderate spending.
3. **High Spenders, High Credit Limit**: Premium customers with high purchasing power.

## Files Included
- **clustered_credit_card_data.csv**: Processed dataset with cluster labels.
- **kmeans_model.pkl**: Saved K-Means model for future use.
- **Python scripts**: Code for data processing, clustering, and visualization.

## How to Use
1. Load the dataset and preprocess it.
2. Train the K-Means model or load the pre-trained model.
3. Use the model to predict customer segments.
4. Implement marketing strategies based on segmentation insights.

## Tools & Libraries Used
- Python
- Pandas
- Matplotlib & Seaborn (for visualization)
- Scipy (for hierarchical clustering)
- Scikit-learn (for K-Means clustering)
- Joblib (for model saving)

## Future Enhancements
- Extend clustering to include more features.
- Apply other clustering techniques like DBSCAN.
- Develop a dashboard for interactive data visualization.
