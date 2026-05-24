<div align="center">

```text
████████╗██╗████████╗ █████╗ ███╗   ██╗██╗ ██████╗ 
╚══██╔══╝██║╚══██╔══╝██╔══██╗████╗  ██║██║██╔════╝ 
   ██║   ██║   ██║   ███████║██╔██╗ ██║██║██║      
   ██║   ██║   ██║   ██╔══██║██║╚██╗██║██║██║      
   ██║   ██║   ██║   ██║  ██║██║ ╚████║██║╚██████╗ 
   ╚═╝   ╚═╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═══╝╚═╝ ╚═════╝


# 🚢 TITANIC SURVIVAL PREDICTION

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-Learn" />
  <img src="https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
  <img src="https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
</p>

> An end-to-end Machine Learning workflow predicting passenger survival on the RMS Titanic.

## 📖 Overview

This project applies machine learning techniques to predict passenger survival on the Titanic. Using the classic Titanic dataset, this notebook demonstrates a complete data science workflow—from data preprocessing and feature scaling to model building and evaluation.

---

## 🛠️ Key Steps & Methodology

### 🧹 1. Data Preprocessing
* **Data Cleaning:** Dropped irrelevant columns (e.g., `deck`, `embark_town`, `who`) to reduce noise.
* **Missing Values:** Handled nulls by imputing the **mean** for the `age` column and completely dropping rows with missing embarkation data.

### 🧬 2. Feature Engineering
* **Categorical Encoding:** Utilized `LabelEncoder` to transform categorical variables (`sex` and `embarked`) into numerical formats understandable by machine learning algorithms.

### ⚖️ 3. Feature Scaling
* **Normalization:** Applied `StandardScaler` to normalize the feature set. This step was crucial for ensuring distance-based models (like KNN) could perform optimally.

### 🤖 4. Model Selection & Training
Built and trained three distinct classification models using **Scikit-Learn**:
* **Logistic Regression**
* **K-Nearest Neighbors (KNN)** *(n_neighbors = 5)*
* **Gaussian Naive Bayes**

---

## 📊 Results & Performance

The models were rigorously evaluated using **accuracy scores**, **confusion matrices**, and **classification reports**. Here is how the models stacked up against one another:

| Model | Accuracy Score |
| :--- | :---: |
| 🏆 **Logistic Regression** | **80.3%** |
| 🥈 **K-Nearest Neighbors (KNN)** | 77.5% |
| 🥈 **Gaussian Naive Bayes** | 77.5% |

---

## 💻 Technologies Used

* **Core Language:** Python
* **Data Manipulation & Analysis:** Pandas, NumPy
* **Data Visualization:** Seaborn *(Dataset loading & visual EDA)*
* **Machine Learning:** Scikit-Learn *(Modeling, Preprocessing, and Metrics)*
