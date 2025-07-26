# Customer-Segmentation
# Overview
This project performs customer segmentation using unsupervised machine learning techniques. By clustering customers based on their annual income and spending score, businesses can better understand and target different customer groups with tailored strategies.

# Dataset
- Source: Kaggle - Mall Customer Segmentation Dataset（https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python）
- File: Mall_Customers.csv
- Key Features:
  - Annual Income (k$)
  - Spending Score (1-100)

# Objectives
- Perform data preprocessing and visual exploration
- Apply K-Means Clustering and determine the optimal number of clusters
- Visualize clustering results using 2D scatter plots
- Try DBSCAN as an alternative clustering method
- Analyze average spending score per cluster

# Tools & Libraries
- Python
- pandas
- matplotlib
- seaborn
- scikit-learn

# Key Steps
- 1. Data Preprocessing
  - Selected only relevant features: Annual Income (k$) and Spending Score (1-100)
  - Scaled data using StandardScaler for optimal clustering performance
- 2. Exploratory Data Analysis
  - Scatter plot to understand the distribution of customers by income and spending
- 3. K-Means Clustering
  - Used the Elbow Method and Silhouette Score to determine the optimal number of clusters
  - Optimal k = 5
  - Visualized customer segments with color-coded scatter plots
- 4. DBSCAN Clustering
  - Used eps=0.5 and min_samples=5
  - Found 2 clusters (excluding noise)
  - Visualized DBSCAN clusters
- 5. Cluster Analysis
  - Calculated average spending scores per cluster for both K-Means and DBSCAN

# Results Summary
- K-Means Clustering
    - Optimal Clusters: 5
    - Cluster Spending Score Means:
      - Cluster 0: 49.52
      - Cluster 1: 82.13
      - Cluster 2: 79.36
      - Cluster 3: 17.11
      - Cluster 4: 20.91
- DBSCAN Clustering
  - Clusters Found: 2 (excluding noise)
  - Cluster Spending Score Means:
    - Cluster 0: 43.10
    - Cluster 1: 82.80
