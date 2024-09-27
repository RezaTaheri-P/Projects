# **Customer Clustering Project**

## **Introduction**

This project focuses on segmenting customers into distinct groups based on their demographic and spending behavior using clustering algorithms. The dataset used in this project contains features like age, income, and spending score. By identifying customer segments, businesses can target marketing strategies more effectively.

### **Dataset Overview**:
- **Number of Examples**: 200 
- **Number of Features**: 5 (including Age, Gender, Annual Income, Spending Score)
- **Objective**: To group customers into meaningful clusters for targeted marketing using clustering algorithms like K-Means, DBSCAN, and Hierarchical Clustering.

## **Algorithms Used**

Several clustering algorithms were implemented to group customers based on the provided features:

1. **K-Means Clustering**
2. **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**
3. **Hierarchical Clustering**

Each algorithm was evaluated using metrics like the **Silhouette Score**, and the results were compared visually.

## **Project Workflow**

### **Step 1: Data Exploration**
- Conducted an initial analysis of the dataset to understand the distribution of customer features such as age, income, and spending score.
- Visualized key features to identify patterns and relationships within the data.

### **Step 2: Data Preprocessing**
- Handled missing data and performed feature scaling to normalize the range of features.
- Encoded categorical variables (like Gender) using label encoding for clustering algorithms to process them.

### **Step 3: Clustering Algorithms**
- **K-Means**: Applied the K-Means algorithm with a predefined number of clusters. Used the elbow method to identify the optimal number of clusters.
- **DBSCAN**: Utilized the K-Distance Graph to determine the appropriate `eps` value for DBSCAN and identified noise (outliers) in the dataset.
- **Hierarchical Clustering**: Created a dendrogram using Agglomerative Clustering to visualize how customer segments are formed and determine the number of clusters.

### **Step 4: Evaluation and Visualization**
- **Silhouette Score**: Evaluated the performance of the clustering algorithms using the Silhouette Score, which measures how well-separated the clusters are.
- **Visualizations**: Plotted clusters for K-Means, DBSCAN, and Hierarchical Clustering to visually compare the segmentation of customers.

### **Model Performance Summary**:

- **K-Means Clustering**:
  - Identified 4 clusters  with a Silhouette Score of 0.4.
  - Visualized clusters based on Age and Spending Score.
  
- **DBSCAN**:
  - Detected core clusters and outliers (noise) in the data using a K-Distance Graph to select `eps`.
  - Silhouette Score: 0.29.

- **Hierarchical Clustering**:
  - Formed customer segments using Agglomerative Clustering and visualized the process with a dendrogram.
  - Silhouette Score: 0.29.

### **Conclusion**

- **K-Means** provided the most balanced clusters based on demographic and spending features, making it the most effective for this dataset.
- **DBSCAN** was particularly useful in identifying outliers or anomalous customers, which could indicate high or low spenders outside the normal range.
- **Hierarchical Clustering** helped visualize the hierarchical relationships between customers but required manual determination of the number of clusters.

### **Business Application**:
The identified clusters can be used by businesses to tailor marketing strategies:
- Target high spenders with loyalty programs.
- Provide discounts to lower-income groups or encourage middle-spenders to increase their purchasing frequency.

## **Future Work**

- Experiment with more advanced clustering techniques, such as **Gaussian Mixture Models**.
- Optimize clustering algorithms using hyperparameter tuning.
- Use dimensionality reduction techniques like PCA to handle higher-dimensional customer data for better cluster separation.

## **Acknowledgments**

- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Matplotlib Documentation](https://matplotlib.org/)
- [Pandas Documentation](https://pandas.pydata.org/)