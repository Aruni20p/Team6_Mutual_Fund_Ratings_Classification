# Team6_Mutual_Fund_Ratings_Classification
# Documentation

# Defining Objective: 
This project aims to apply Clustering based on features such as tempo, loudness and danceability. These insights in future will help the creation of personalized music recommendations tailored to individual emotional needs, enhancing the effectiveness of music-based interventions.

# Importing Necessary Libraries
# Data Acquisition: 
The dataset contains 12 features and 5235 including some important and some redundant.

# Data Preprocessing: 
We performed a rigorous Data Preprocessing to improve quality of the clusters formed. 

# Model Selection for Clustering
1.) K-Means: When the number of clusters is known in advance, and the data is expected to form spherical clusters.

2.) Hierarchical: It is also useful when visualizing clusters through a dendrogram.

3.) DBSCAN: When the clusters have arbitrary shapes, and you want to identify noise or outliers in the data. It is useful for datasets with varying density or for spatial data.

# Evaluation:
1.) Silhouette Score-: Measures how similar a data point is to its own cluster (cohesion) compared to other clusters (separation).
2.)The Davies-Bouldin Index (DBI)-: It is a metric that evaluates cluster separation by comparing the intra-cluster distance with the inter-cluster distance. It measures how well-separated the clusters are.
3.) The Calinski-Harabasz Index-: It measures the ratio of the sum of between-cluster dispersion to within-cluster dispersion.

