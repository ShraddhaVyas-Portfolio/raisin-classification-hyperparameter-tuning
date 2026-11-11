Raisin Classification with Hyperparameter Tuning
Project Overview
This machine learning project classifies two raisin varieties, Kecimen and Besni, using morphological measurements from the Raisin Dataset.

The project demonstrates the use of machine learning classification techniques and hyperparameter optimization to improve model performance.

Dataset
Source: Kaggle Raisin Dataset

Total Samples: 900
Features: 7 numerical features
Target Variable: Class (Kecimen or Besni)
Features include:

Area
MajorAxisLength
MinorAxisLength
Eccentricity
ConvexArea
Extent
Perimeter
Technologies Used
Python
Pandas
NumPy
Scikit-Learn
SciPy
Jupyter Notebook
Project Workflow
1. Data Preparation
Loaded and explored the dataset
Created predictor variables (X)
Created target variable (y)
Split data into training and testing sets
2. Decision Tree Classification
Implemented:

DecisionTreeClassifier()
Hyperparameters tuned using:

GridSearchCV()
Parameters tested:

max_depth = [3, 5, 7]
min_samples_split = [2, 3, 4]
3. Logistic Regression Classification
Implemented:

LogisticRegression(
    solver='liblinear',
    max_iter=1000
)
Hyperparameters tuned using:

RandomizedSearchCV()
Parameters searched:

penalty = ['l1', 'l2']
C = Uniform Distribution (0-100)
Best Logistic Regression Results
Metric	Value
Penalty	L2
C Value	4.65
Cross Validation Accuracy	87.08%
Test Accuracy	84.44%
Best Model:

LogisticRegression(
    C=4.647392931567273,
    penalty='l2',
    solver='liblinear',
    max_iter=1000
)
Skills Demonstrated
Machine Learning Classification
Hyperparameter Tuning
Grid Search CV
Randomized Search CV
Logistic Regression
Decision Trees
Model Evaluation
Scikit-Learn
Future Improvements
Try Support Vector Machines (SVM)
Experiment with K-Nearest Neighbors (KNN)
Implement Gradient Boosting Models
Perform Feature Engineering
Improve model performance through additional tuning
Author
Shraddha Vyas

GitHub Portfolio: https://github.com/ShraddhaVyas-Portfolio
