 Team6_Mutual_Fund_Ratings_Classification
# Documentation


# Defining Objective: 

The rating serves as a measure of the fund's overall performance, risk, sustainability, and other financial metrics. We aim to predict the rating of a mutual fund based on various factors related to its investment strategy, financial ratios, historical returns, and ESG (Environmental, Social, and Governance) factors.
This project aims to apply Clustering based on features such as tempo, loudness and danceability. These insights in future will help the creation of personalized music recommendations tailored to individual emotional needs, enhancing the effectiveness of music-based interventions.

# Importing Necessary Libraries
# Data Acquisition: 
The dataset contains 132 features including some important and some redundant and target variable i.e. rating
# Data Preprocessing and EDA: 
We performed a rigorous Data Preprocessing via exploratory data analysis. To enhance the performance of our model  we performed PCA, added new features
The dataset contains 12 features and 5235 including some important and some redundant.

# Data Preprocessing: 
We performed a rigorous Data Preprocessing to improve quality of the clusters formed. 

# Model Selection for Clustering
K-Means: When the number of clusters is known in advance, and the data is expected to form spherical clusters.

# Train-Validation-Test Split:
Our data is split into 80:10:10, training set has 80%, validation size (10%), and test 10% of the sets, ensuring models are rigorously evaluated.
Hierarchical: It is also useful when visualizing clusters through a dendrogram.

# Model Selection
Since our classes our imbalanced we tried different techniques to address it. SMOTE and SMOTEEN are both techniques used to address the issue of class imbalance in datasets. SMOTE does not change the majority class and does not address the issue of potential "noise" in the majority class. y combining the generation of synthetic minority examples (SMOTE) with the removal of noisy samples (ENN), SMOTEEN can help to create a more distinct and accurate decision boundary between the minority and majority classes.
After rigorous walkthrough and much reasoning, we selected and implemented three tree based models for ratings classification on the balanced dataset:
1.	Random Forest: Multiple decision trees are built on random subsets of the data, and their predictions are averaged to improve accuracy and reduce overfitting.
2.	XGBoost: A series of decision trees are built sequentially, each one correcting the errors of the previous one, using a boosting approach.
3.	LightGBM: Similar to XGBoost, but uses a histogram-based approach and leaf-wise tree growth, making it faster and more efficient on large datasets..
DBSCAN: When the clusters have arbitrary shapes, and you want to identify noise or outliers in the data. It is useful for datasets with varying density or for spatial data.

# Evaluation:
Precision is important in this context because it ensures the reliability of our model when predicting mutual fund ratings, helping avoid serious errors that could mislead investors or impact trust.

## Dataset Source
https://www.kaggle.com/datasets/stefanoleone992/european-funds-dataset-from-morningstar
