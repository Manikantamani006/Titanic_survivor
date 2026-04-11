Titanic Survival Prediction
Overview
This project applies machine learning techniques to predict passenger survival on the Titanic. Using the classic Titanic dataset, this notebook demonstrates a complete end-to-end data science workflow, from data preprocessing and feature scaling to model building and evaluation.

Key Steps & Methodology
Data Preprocessing: Cleaned the dataset by dropping irrelevant columns (e.g., deck, embark_town, who), handling missing values (imputing the mean for the age column), and removing rows with missing embarkation data.

Feature Engineering: Used LabelEncoder to transform categorical variables (sex and embarked) into numerical formats suitable for machine learning algorithms.

Data Scaling: Applied StandardScaler to normalize the feature set, ensuring models like KNN could perform optimally.

Model Selection & Training: Built and trained three different classification models using scikit-learn:

Logistic Regression * K-Nearest Neighbors (KNN) (n_neighbors = 5)

Gaussian Naive Bayes

Results
The models were evaluated using accuracy scores, confusion matrices, and classification reports.

Logistic Regression: Achieved the highest accuracy at 80.3%.

K-Nearest Neighbors (KNN): Achieved an accuracy of 77.5%.

Gaussian Naive Bayes: Achieved an accuracy of 77.5%.

Technologies Used
Python

Libraries: Pandas, NumPy, Seaborn (for dataset loading), Scikit-learn (for modeling, preprocessing, and metrics)
