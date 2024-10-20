# Team6_Mutual_Fund_Ratings_Classification
# Documentation


# Defining Objective: 

The rating serves as a measure of the fund's overall performance, risk, sustainability, and other financial metrics. We aim to predict the rating of a mutual fund based on various factors related to its investment strategy, financial ratios, historical returns, and ESG (Environmental, Social, and Governance) factors.

# Importing Necessary Libraries
# Data Acquisition: 
The dataset contains 132 features including some important and some redundant and target variable i.e. rating
# Data Preprocessing and EDA: 
We performed a rigorous Data Preprocessing via exploratory data analysis. To enhance the performance of our model  we performed PCA, added new features

# Train-Validation-Test Split:
Our data is split into 80:10:10, training set has 80%, validation size (10%), and test 10% of the sets, ensuring models are rigorously evaluated.

# Model Selection
Since our classes our imbalanced we tried different techniques to address it. SMOTE and SMOTEEN are both techniques used to address the issue of class imbalance in datasets. SMOTE does not change the majority class and does not address the issue of potential "noise" in the majority class. y combining the generation of synthetic minority examples (SMOTE) with the removal of noisy samples (ENN), SMOTEEN can help to create a more distinct and accurate decision boundary between the minority and majority classes.
After rigorous walkthrough and much reasoning, we selected and implemented three tree based models for ratings classification on the balanced dataset:
1.	Random Forest: Multiple decision trees are built on random subsets of the data, and their predictions are averaged to improve accuracy and reduce overfitting.
2.	XGBoost: A series of decision trees are built sequentially, each one correcting the errors of the previous one, using a boosting approach.
3.	LightGBM: Similar to XGBoost, but uses a histogram-based approach and leaf-wise tree growth, making it faster and more efficient on large datasets..

# Evaluation:
Precision is important in this context because it ensures the reliability of our model when predicting mutual fund ratings, helping avoid serious errors that could mislead investors or impact trust.

