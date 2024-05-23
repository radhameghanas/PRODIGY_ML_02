# PRODIGY_ML_02
Synopsis of the Code
1. Importing Libraries:

Various Python libraries for data manipulation, visualization, and machine learning are imported, including numpy, pandas, matplotlib.pyplot, seaborn, plotly, and KMeans from sklearn.cluster.
Warnings are suppressed, and operating system functionality is imported.

2. Data Exploration:

The dataset Mall_Customers.csv is loaded into a DataFrame named df.
The first few rows, shape, summary statistics, data types, and missing values of the dataset are displayed.
The dataset consists of 200 entries with columns: CustomerID, Gender, Age, Annual Income (k$), and Spending Score (1-100).

3. Data Visualization:

Histograms:
  Distribution plots for Age, Annual Income (k$), and Spending Score (1-100) are created using Seaborn.
Count Plot of Gender:
  A count plot showing the distribution of Gender is created.
Relationships between Variables:
  Scatter plots and regression plots to show relationships between Age, Annual Income (k$), and Spending Score (1-100) are generated.
  Scatter plots for Age vs Annual Income and Annual Income vs Spending Score are plotted, differentiated by Gender.
  Violin and swarm plots show the distribution of Age, Annual Income, and Spending Score according to Gender.
  
4. Clustering using K-Means:

Segmentation using Age and Spending Score:
  K-Means clustering is applied on Age and Spending Score (1-100).
  The optimal number of clusters is determined using the elbow method.
  A K-Means model with 4 clusters is trained, and the clusters are visualized.
Segmentation using Annual Income and Spending Score:
  K-Means clustering is applied on Annual Income (k$) and Spending Score (1-100).
  The optimal number of clusters is determined using the elbow method.
  A K-Means model with 5 clusters is trained, and the clusters are visualized.
Segmentation using Age, Annual Income, and Spending Score:
  K-Means clustering is applied on Age, Annual Income (k$), and Spending Score (1-100).
  The optimal number of clusters is determined using the elbow method.
  A K-Means model with 6 clusters is trained, and the clusters are visualized in a 3D plot using Plotly.
  
5. Model Building:

Feature Selection:
  The features Annual Income (k$) and Spending Score (1-100) are selected for model building.
Optimal Cluster Number:
  The elbow method is used again to determine that 5 clusters are optimal.
Final K-Means Model:
  A final K-Means model with 5 clusters is built and fitted to the data.
  The clusters are visualized in a 2D scatter plot, showing the centroids.
  
6. Model Interpretation:

The clusters are interpreted as follows:
Cluster 1: High income, low spending.
Cluster 2: Average income and spending.
Cluster 3: High income, high spending (target customers).
Cluster 4: Low income, high spending.
Cluster 5: Low income, low spending.
